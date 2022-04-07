
# Rapport

Följde stegen:
Navigerade till res-values-strings där ändrade jag värdet i appname
Navigerade till app-manifest-AndroidManifest och la in ```<uses-permission android:name="android.permission.INTERNET" />```
Bytte ut textView til webView i content_main
I WebView ```android:id="@+id/my_webview"``` för att ge webviewen ett unikt id
I MainActivity under onCreate ```myWebView = findViewById(R.id.my_webview);
                                         myWebView.getSettings().setJavaScriptEnabled(true);```
Detta kallar på min webview när appen startas och enablar javascript
Själva myWebView variabeln skapas direkt under classen mainactivity
Lade till en intern sida som asset i en directory folder - assets-img-about.html
Ordnade så att variablerna showInternalWebPage och showExternalWebPage kör funktionen getUrl
``` myWebView.loadUrl("file:///android_asset/img/about.html");```


![](Android.png)
