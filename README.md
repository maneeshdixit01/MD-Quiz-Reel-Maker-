# MD Quiz Reel Maker (v8.0 — Large MP4 Save & Share Fixed)

Instagram Reels, Facebook Reels, YouTube Shorts (9:16) और सामान्य YouTube वीडियो (16:9 लैंडस्केप) बनाने का पूरा वेब व Android (Capacitor) प्रोजेक्ट।

## v8.0 में सुधारी गई समस्याएँ
- **बड़े वीडियो (30–200 MB) का भरोसेमंद डाउनलोड (Chunked Save):** Android APK में `Filesystem.writeFile` + `appendFile` द्वारा वीडियो को 768 KB के सुरक्षित हिस्सों में लाइव प्रोग्रेस बार के साथ `Documents/MD_Quiz_Videos` में सेव किया जाता है, जिससे 10–20 प्रश्नों की बड़ी वीडियो कभी फेल नहीं होती।
- **शेयर बटन फिक्स (APK + Chrome दोनों में):** MIME टाइप से `;codecs=...` हटाकर साफ `video/mp4` सेट किया गया है और Android Capacitor Share v6 के `files: [uri]` सपोर्ट के साथ चंक्ड कैश सेविंग जोड़ी गई है।
- **संतुलित MP4 साइज:** 1080p के लिए स्मार्ट बिटरेट (`2.6 Mbps` संतुलित, `4.5 Mbps` Ultra और `1.6 Mbps` 720p) ताकि वीडियो साफ भी रहे और साइज लगभग आधा होकर तेज़ी से सेव/अपलोड हो।
