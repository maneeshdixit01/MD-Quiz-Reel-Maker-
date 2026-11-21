# MD Quiz Reel Maker (v10.0 — Standard MP4 Gallery Remuxer + Native Hindi TTS)

Instagram Reels, Facebook Reels, YouTube Shorts (9:16) और सामान्य YouTube वीडियो (16:9 लैंडस्केप) बनाने का पूरा वेब और Android (Capacitor) प्रोजेक्ट।

## v10.0 में किया गया बड़ा सुधार (1-सेकंड ड्यूरेशन बग का स्थायी निदान)
- **ऑटोमैटिक लॉसलेस MP4 रिमक्सिंग (`VideoFixerPlugin.java`):** Android के नेटिव `MediaExtractor` और `MediaMuxer` से फ्रेगमेंटेड MP4 को 1–2 सेकंड में बिना क्वालिटी घटाए मानक (Standard) MP4 में बदल दिया जाता है।
- **सीधे फोन की गैलरी में सेव (`Movies/MD_Quiz_Videos`):** Android `MediaStore` के ज़रिए वीडियो असली कुल लंबाई (`DURATION`) के साथ सीधे गैलरी में दिखता है और बिना WhatsApp पर भेजे सीधे Instagram, Facebook व YouTube पर अपलोड हो जाता है।
- **ब्राउज़र के लिए इन-प्लेस हेडर फिक्सर:** Chrome में सीधे चलाने पर भी MP4 के `mvhd`/`tkhd`/`mdhd`/`mehd` हेडर में असली लंबाई तुरंत लिख दी जाती है।
- **Google Maven Mirror + Native Android Hindi TTS** पहले से शामिल हैं।
