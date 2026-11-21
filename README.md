# MD Quiz Reel Maker (v9.0 — Native Android Hindi TTS + Direct MP4 Mixing)

Instagram Reels, Facebook Reels, YouTube Shorts (9:16) और सामान्य YouTube वीडियो (16:9 लैंडस्केप) बनाने का पूरा वेब और Android (Capacitor) प्रोजेक्ट।

## v9.0 में नए सुधार
- **Android APK के अंदर नेटिव हिंदी TTS (`NativeTtsPlugin.java`):** अब Android WebView में "कंप्यूटर स्पीच उपलब्ध नहीं है" वाली त्रुटि हमेशा के लिए खत्म हो गई है। ऐप सीधे फोन के Google/Android Text-to-Speech इंजन से हिंदी में बोलता है।
- **बिना माइक के MP4 वीडियो में हिंदी आवाज़:** MP4 वीडियो बनाते समय Android नेटिव TTS हर प्रश्न, सही उत्तर और अंतिम संदेश की साफ `.wav` आवाज़ बनाकर सीधे वीडियो के ऑडियो ट्रैक में मिक्स कर देता है (कोई बाहरी शोर नहीं, और आवाज़ की असली लंबाई के अनुसार टाइमर बिल्कुल सटीक चलता है)।
- **आसान GitHub अपलोड:** `NativeTtsPlugin.java` और `MainActivity.java` को रूट फोल्डर में ही रखा गया है; `build-android.yml` उन्हें अपने-आप Android प्रोजेक्ट में लगाकर और Android 11+ `TTS_SERVICE` क्वेरी जोड़कर APK बिल्ड कर देता है।
