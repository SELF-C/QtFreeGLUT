# QtFreeGLUT
Qt + FreeGLUT のOpenGLで描画

glutでティーポットを描画しようとすると`fghDrawGeometryWire`のカレントウインドウを取得するコードでNULLポインタ アクセスしていた。
glutCreateWindow()とかでウインドウを開かない限り、値がセットされないらしい。
Qtからプリミティブの描画だけ行うにはソースを修正する必要がある？

http://tanehp.ec-net.jp/heppoko-lab/diary/d2014_12.html
