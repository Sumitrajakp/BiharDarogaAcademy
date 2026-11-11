# Bihar Daroga Academy — Android MVP

## फोन से APK बनाने का तरीका (बिना कंप्यूटर)

इस प्रोजेक्ट में `.github/workflows/android.yml` दिया गया है। GitHub Actions क्लाउड में Android APK बनाएगा।

1. फोन के Chrome में GitHub खोलें और अकाउंट बनाएँ/साइन इन करें।
2. `New repository` बनाएँ। नाम रखें `BiharDarogaAcademy` और visibility **Public** चुनें (GitHub Actions के मुफ्त उपयोग को सरल रखने के लिए)। इसमें निजी जानकारी न रखें।
3. इस ZIP को फोन में Extract करें। GitHub वेबसाइट पर repository में `Add file` → `Upload files` चुनें और Extract किए गए फ़ोल्डर की सभी फाइलें/फ़ोल्डर अपलोड करें। `.github` फ़ोल्डर भी अपलोड होना जरूरी है।
4. `Commit changes` करें। `Actions` टैब खोलें। `Build Android APK` workflow अपने-आप शुरू होगा; जरूरत हो तो `Run workflow` दबाएँ।
5. Build सफल होने पर workflow run खोलें। नीचे `Artifacts` में `Bihar-Daroga-Academy-debug-apk` डाउनलोड करें।
6. ZIP artifact Extract करें। `app-debug.apk` खोलकर इंस्टॉल करें। Android पूछे तो केवल इसी अपने बनाए APK के लिए browser/files app को install permission दें।

## जरूरी बातें
- यह debug APK है, Play Store release नहीं।
- GitHub अकाउंट और इंटरनेट जरूरी हैं; फोन पर Android Studio की जरूरत नहीं।
- GitHub UI मोबाइल ब्राउज़र पर थोड़ा कठिन हो सकता है; Chrome में Desktop site चालू करना मदद कर सकता है।
- सार्वजनिक repository में कोई निजी जानकारी, पासवर्ड या API key न डालें।
- यह MVP demo है; पूर्ण पाठ्यक्रम, वास्तविक PYQ बैंक, notifications, cloud sync और user login अभी विकसित होने बाकी हैं।
- ऐप की डेमो क्लास/क्विज़ और स्थानीय progress ऑफलाइन चलती है।
