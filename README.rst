iphoneからMacのマウスを操作する
 =================================
 =================================
 
 
-あとでちゃんとかくかも。
 
 
+対象環境
+=========
+* mac os x 10.8.2
+* python 2.7.3
+* virtualenv
+* mkvirtualenv
 
 
-how to use
+
+準備
 ==========
 ==========
-1. いろいろと必要なライブラリをインストールする。
+flask, tornadoをインストールします。
-2. templates/index.htmlの10.1.2.240をPCのIPに変更。
+::
-3. terminal 1: python ws_server.py
+
-4. terminal 2: python http_server.py
+    mkvirtualenv controlmouse
-5. iphoneで 2で書き換えたIP:5000にアクセス。
+    pip install flask
-6. ぐりぐりするとマウスが動く。
+    pip install tornado
+
+
+実行
+====
+
+1. terminalを２つ起動しておきます。
+2. terminalの１つ目::
+
+    cd controlmouse/app
+    workon controlmouse
+    python http_server.py
+
+3. terminalの２つ目::
+
+    cd controlmouse/app
+    workon controlmouse
+    python ws_server.py
+
+4. iphoneのsafariで http://MacのIP:5000/ を開く。
 
 
 
 
