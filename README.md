# ラズベリーパイによる手書き入力の研究
Raspery Piとは
ラズベリーパイの導入
１６ＧＢのメモリーカード、ラズベリーパイ、

processingの導入

>void setup() { size(640, 360); background(102); } 
>void draw() { stroke(255); if (mousePressed==true){
>line(mouseX, mouseY, pmouseX, pmouseY); } 
}
int count = 1 ;
void keyPressed(){
  if(key == 'p' || key == 'P'){
    String path  = System.getProperty("user.home") + "/Desktop/scereenshot" + count + ".jpg";
    save(path);
    count++;
    println("screen saved." + path);
  }
}
