# 🔐 Hooza ( Quiz Game)
Hooza คือ โปรแกรมที่ไว้ใช้สำหรับการสร้างคำถามต่าง ๆ เพื่อใช้กับเรื่องต่าง ๆไม่ว่าจะเป็น การทบทวนคำถามหลังเรียน, การใช้ในการสอบ ฯลฯ โดยตัวโปรแกรมจะแบ่งออกเป็น 2 ส่วนคือ `Teacher` และ `Student` ในส่วนของ `Teacher` จะมีตัวเลือกสำหรับการสร้างคำถามและการสร้าง Lobby ซึ่งส่วนของ `Student` จะมีการ Join เข้าสู่ Lobby ของ `Teacher` เท่านั้นโดยจะ Join เข้าไปที่ IP ของ `Teacher`

*** สำหรับรหัสในการใช้งานช่วงพัฒนานั้น *** <br>
`Teacher` คือ Username : `0001`     Password : `1234` <br>
`Student` คือ Username : `60070003`  Password : `1234`

*** ผู้ใช้งานทั้งหมดจำเป็นต้องเชื่อมต่อภายใน Network เดียวกัน ***
## ภาษาที่ใช้ในการพัฒนา Hooza
<img src="http://www.digitaltrends.com/wp-content/uploads/2010/11/java-logo.jpg" >

# 🗜️ขั้นตอนในการลง Libraries?
## *** หากต้องการที่จะใช้งานตัวโปรแกรมโดยไม่จำเป็นต้องเพิ่ม Libraries สามารถทำได้โดยการ Clone ตัว project แล้วใช้งานตัวโปรแกรมผ่าน Folder JAR และ                    รันตัว _Hooza.jar ***
## 🤖ขั้นตอนในการเพิ่ม Libraies🤖
- File -> Project Structure
<img src="https://scontent.fbkk22-2.fna.fbcdn.net/v/t1.0-9/48367275_2255896331144845_8466258152558428160_o.jpg?_nc_cat=107&_nc_eui2=AeHU_EKVOAtV8R176qw6R_CdNeKgxvKJ8IyYBc1lMDGLfvHWG3Xxuaf2g9cXO1RdolST7fFyWKZ2BNDoXJm3oBfKtMO9M3s59QyD4e_bT65Iqw&_nc_ht=scontent.fbkk22-2.fna&oh=e64b6da30b983fab82c6107550ea54eb&oe=5C94A42F" width="800"/>
<img src="https://scontent.fbkk22-1.fna.fbcdn.net/v/t1.0-9/48421999_2255896254478186_5699466720423444480_o.jpg?_nc_cat=110&_nc_eui2=AeGM6YpCrEtbnNnTWW1oPB_jm8LBtETSR9I66MZ7L84bm7I5iyXtW1Fhb9gMVTf4N29xFA9an8rNmXPCgc9eb7Ib83cxGolNzZLu_l9OD8yXDg&_nc_ht=scontent.fbkk22-1.fna&oh=e384ee5b932c762479b8b82f474589f9&oe=5C93C281" width="800"/>
<img src="https://scontent.fbkk22-2.fna.fbcdn.net/v/t1.0-9/48416376_2255896277811517_6366148792697225216_o.jpg?_nc_cat=109&_nc_eui2=AeG7v3K_YQ1c2rL5_UWQGWjlKeLLyroMSfCEwad54AJW7Wm-WiDMTceEVQ9kwW6XIgr01rTGpNB0X0ArIqo_aaI74UogB0v5w2SzEiEQiMaO2Q&_nc_ht=scontent.fbkk22-2.fna&oh=a628f13a1a3a8fc5dd2d9533f1b22374&oe=5C93C795" width="800"/>



# 🗜️ขั้นตอนการทำงานของ Hooza?

1.) เมื่อเปิดโปรแกรมขึ้นมาแล้วจะพบกับหน้าเข้าสู่ระบบ ซึ่งข้อมูลของผู้ใช้ต่าง ๆ ไม่ว่าจะเป็น ชื่อ, นามสกุล, รหัสนักศึกษา, คะแนน จะถูกเก็บอยู่บน Database Online ซึ่งจะต้องเพิ่ม Library สำหรับการเชื่อมต่อ Database ซึ่ง Library เมื่อ Clone Project มาแล้วจะมาพร้อมกับ `mysql-connector-java-8.0.13.jar` ซึ่งเป็น Library สำหรับการเชื่อม Database

<p float="left">
  <img src="https://scontent.fbkk2-8.fna.fbcdn.net/v/t1.0-9/48359393_2254579374609874_111344196765351936_o.jpg?_nc_cat=104&_nc_ht=scontent.fbkk2-8.fna&oh=ada65ba41a8036e66bba9edd40338af8&oe=5CAA8492" width="800"/>
</p>


<p float="left">
  <img src="https://scontent.fbkk2-7.fna.fbcdn.net/v/t1.0-9/48364335_2254579351276543_5104517796063084544_n.jpg?_nc_cat=106&_nc_ht=scontent.fbkk2-7.fna&oh=0b5148baabd3769684edee5a1c8262b8&oe=5C9A687F" width="300" /> 
  <img src="https://scontent.fbkk1-4.fna.fbcdn.net/v/t1.0-9/48394149_2255541967846948_5148722999632855040_n.jpg?_nc_cat=105&_nc_eui2=AeFQVQohe_FD0Xh5hvdYKru-nMvh2pu8s1n_8JLNIOWyDywjf_qLrO-TPngpkEprkoQah4AdjKXWiRu6GAcDKy0P-YW02amRC1p14bTI5dzkAg&_nc_ht=scontent.fbkk1-4.fna&oh=eb20fa8c6604b8d697c9996e0e34444a&oe=5CA66FB4" width="300" />
</p>


2.) หลังจากเข้าสู่ระบบเรียบร้อยแล้วหน้าต่างของ `Teacher` และ `Student` จะมีความแตกต่างกันตรงที่ `Teacher` จะมีหน้าต่าง Quiz editor กับ Create room เพิ่มขึ้นมา

<p float="left">
  <img src="https://scontent.fbkk2-7.fna.fbcdn.net/v/t1.0-9/48369221_2254579357943209_6639710936410095616_n.jpg?_nc_cat=106&_nc_ht=scontent.fbkk2-7.fna&oh=5c553a1be972507be97e3dfaeefc2e61&oe=5C91DF4D" width="300" /> 
  <img src="https://scontent.fbkk1-5.fna.fbcdn.net/v/t1.0-9/48373824_2255547104513101_4051158576884875264_n.jpg?_nc_cat=111&_nc_eui2=AeGZA4UJkKZhH4NQZF9WHgkrK0REn2FDOk_Wu3_GDY8XuCO266MjJkbW8tKlR2Z7_7Oe1LOqHStgFM57iUcA1gukGQaXcMxvLCNfVNrIL1JLbQ&_nc_ht=scontent.fbkk1-5.fna&oh=26a481b1fffc3e8bc0d621b8eeeddd29&oe=5CD76145" width="300" height="485"/>
</p>

3.) ในส่วนการทำงานใน Quiz editor นั้นจะมีไว้สำหรับการสร้างคำถาม ในส่วนของคำถามนั้นจะมีการบันทึกไฟล์เก็บไว้ในตัวเครื่องเป็น Object ของคำถาม ใน Quiz 1 ข้อ สามารถสร้างข้อย่อยได้หลายข้อ เมื่อเราสร้างคำถามแล้ว ให้กด add problem เพื่อเพิ่มคำถามเข้าไปใน Quiz และเราสามารถเก็บคำถามได้มากกว่า 1 คำถาม หลังจากนั้นเมื่อเพิ่มคำถามตามจำนวนที่ต้องการแล้วก็ให้กด Save Quiz เพื่อบันทึก Quiz ลงในเครื่อง

<p float="left">
  <img src="https://scontent.fbkk2-7.fna.fbcdn.net/v/t1.0-9/48391412_2254579417943203_686741957547917312_o.jpg?_nc_cat=111&_nc_ht=scontent.fbkk2-7.fna&oh=ac25989ee5d34f06f01ef2521686851a&oe=5CA51200" width="300" /> 
  <img src="https://scontent.fbkk1-6.fna.fbcdn.net/v/t1.0-9/48370488_2255552624512549_81057272804933632_n.jpg?_nc_cat=104&_nc_eui2=AeGpLOGdYq5POeSuJCPmdExU1qzApEwpsm-nITvs1Z96dpzeYOE1ZMnaE868ZPBlAd3BlsrvV7vzAxWBywlQcFM38MrQr3hGic_nFIPILEIsiA&_nc_ht=scontent.fbkk1-6.fna&oh=37db327089f0de952b3eed4992429b34&oe=5CA2456F" width="300"/>
</p>

4.) หลังจากที่สร้างคำถามเสร็จเรียบร้อยแล้ว ในส่วนของ `Teacher` ต้องทำการสร้าง Lobby เพื่อให้ `Student` เชื่อมต่อเข้ามา การทำงานของ `Hooza` นั้นจะมีการทำงานผ่านทาง Socket เมื่อ `Teacher` สร้าง Lobby จะเป็นการสร้างตัว Server เพื่อไว้ใช้สำหรับการเชื่อมต่อระหว่าง `Student` และ `Teacher` ซึ่งตัว Server จะแตก Thread ให้แก่ตัว `Student` ทุกตัวที่เชื่อมต่อเข้ามาที่ Lobby
หลังจาก `Teacher` เข้าสู่หน้าต่าง Create room แล้วจะต้องทำการกดปุ่ม `Open` เพื่อเป็นการโหลดคำถามที่ได้สร้างขึ้นจากตัวเครื่อง จากนั้นกดปุ่ม Start เพื่อเริ่มเล่น หลังจากกดปุ่ม Start แล้วปุ่มจะเปลี่ยนเป็นปุ่ม Next เพื่อไว้ใช้สำหรับกดไปในข้อถัดไป, ปุ่ม Stop สำหรับการหยุด Quiz ในข้อนั้นและแสดงผลว่ามีใครตอบข้อใดบ้างและข้อใดที่ถูก

<p float="left">
  <img src="https://scontent.fbkk1-3.fna.fbcdn.net/v/t1.0-9/48403839_2255559811178497_9222671115371937792_n.jpg?_nc_cat=109&_nc_eui2=AeF0b9ys06PuOxL7Tnhq5QsBZb3zz-S1EZcBPknn9kU6-rxq3th1IDROR3K0sw6Ycd1chdfwzIAueEcVztTwhnKvVAyu39PAgW6ZjbEcx0x0MA&_nc_ht=scontent.fbkk1-3.fna&oh=d1d6bd4a85f42491c7bbca58f17850b6&oe=5C8B6502" width="300" /> 
  <img src="https://scontent.fbkk1-1.fna.fbcdn.net/v/t1.0-9/48989508_2255547121179766_2146673728837124096_n.jpg?_nc_cat=103&_nc_eui2=AeHP3t-35znHKNq4FlVwA1AB2_pghvCmuSfc0xxkCK83kWEG9RIHKjeZJ8SeTZhaMhahGuuS2HYXouRr02X7-pl7Ri5rR6wwaiRaORKOqYVaxg&_nc_ht=scontent.fbkk1-1.fna&oh=cca0558bbf1a74624473f3f821de2ed7&oe=5CD6B136" width="300"/>
</p>

5.) หลังจากที่ `Student` Join เข้าสู่ Lobbyโดยใช้ Ip ที่แสดงอยู่ในส่วนของ Server แล้ว `Teacher` สามารถตรวจสอบได้ว่ามี `Student` คนไหนเข้ามาแล้วบ้าง หลังจากที่ `Teacher` กด Start แล้วจะมีการส่งคำถามไปทีละข้อให้กับ `Student` แต่ละคน
เมื่อ `Student` ทุกคนตอบคำถามเสร็จแล้วในข้อนั้นหรือเวลาหมด ฝั่ง `Teacher` จะทำการกด Stop เพื่อเป็นการสิ้นสุดคำถามในข้อนั้นแล้วจะแสดงหน้าต่างกราฟแสดงว่า มีใครตอบข้อไหนบ้างแล้วข้อที่ถูกคือข้อไหน
เมื่อตอบคำถามครบทุกข้อแล้ว จะมีหน้าต่างแสดงว่า ได้คะแนนทั้งหมดเท่าไรและมีคะแนนรวมทั้งหมดเท่าไรแล้ว
จะทำการเก็บคะแนนนั้นไว้ที่ Database

<p float="left">
  <img src="https://scontent.fbkk1-5.fna.fbcdn.net/v/t1.0-9/48366829_2255560801178398_8337683590678577152_o.jpg?_nc_cat=102&_nc_eui2=AeFXkoZ9NOwMTjhYqNg4u-Dnp_eLLSmhtXmKT19seEy7qZ-fWFLhPDA3V8DqE_NpFe9sm-WNp2kK6pXkpHPtjMGBEMbLD7npRo2aHjVng6gP_A&_nc_ht=scontent.fbkk1-5.fna&oh=ca53f044bd227bffcc6c2aa3871ae7e4&oe=5CA00BE7" width="300" /> 
  <img src="https://scontent.fbkk1-6.fna.fbcdn.net/v/t1.0-9/48359406_2255560841178394_4067923535048212480_o.jpg?_nc_cat=104&_nc_eui2=AeFHoD5eT6nn6WzNGb8iDIL-RghvwqHzqjcPHQpNyjtrKhgyfsl_7IAdMvD11lBTeS1OGfb1A4r6mxTjeES0zdWI82MoO30c1nVTrEksfjjooQ&_nc_ht=scontent.fbkk1-6.fna&oh=86d7bdc96c220719e72b4e787c860706&oe=5CD86C9F" width="300"/>
</p>

<p float="left">
  <img src="https://scontent.fbkk1-6.fna.fbcdn.net/v/t1.0-9/48377623_2255560834511728_6559128691283066880_o.jpg?_nc_cat=104&_nc_eui2=AeEuT5cw0RElePgSOJdWN2PEc8SAW4C2L8dRiofh4DUQqLkOsksIdkcI5Nx1BiTlOV1KrEX3sySJ04Kr_AcB3DO29sEmi7MDEgXkTFtJ1e4XJg&_nc_ht=scontent.fbkk1-6.fna&oh=5541fd1543dfa68bd0fe1d38b49bea8a&oe=5C9AE73D" width="300" /> 
  <img src="https://scontent.fbkk1-5.fna.fbcdn.net/v/t1.0-9/48425735_2255563984511413_1828529858951512064_o.jpg?_nc_cat=111&_nc_eui2=AeEcWGdPI-BBpzTamIDk5hX2ZAf5arCxSaxMMXbea942iaa-ew0uoM7e-S0Fc_i_vE9vmOYKnNaoH_fIFdJ9b61RNWIq6QCAgfEA8Xs7dhFD9Q&_nc_ht=scontent.fbkk1-5.fna&oh=07cc54f03903f87bce615afc7923b7b4&oe=5CD63477" width="300"/>
</p>



### ตัวอย่าง Code ของ การสร้าง Socket ของ Server
```java
public void run(){

        try {
            ss = new ServerSocket(5555);
            System.out.println("Server is running..");
            analysis = new QuestionAnalysis();
            while (!exit){
                client = new Clienthanler(ss.accept());
                client.setQuestionAna(analysis);
                tr = new Thread(client);  //tr stand for Thread
                tr.start();
                list.add(client);
                try{
                    Thread.sleep(10);
                    ta.append(client.getID() + "\n");
                }catch (Exception ex){
                    System.out.println("Thread sleep error :" + ex);
                }
            }
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
```
### ตัวอย่าง Code ของการจัดการกับ Student แต่ละคน
``` java
    public void run() {

        String run = "";
        //read input only
        try {
            while(running){
                run = in.readLine();
                System.out.println(run);
                String[] data = run.split(" ");
                if(data[0].equals("id")){
                    ID = data[1];
                }
                else if(data[0].equals("ch")){

                    if(data[1].equals("A")){
                        analysis.SetA();
                    }
                    else if(data[1].equals("B")){
                        analysis.SetB();
                    }
                    else if(data[1].equals("C")){
                        analysis.SetC();
                    }
                    else if(data[1].equals("D")){
                        analysis.SetD();
                    }

                }
            }

        }
        catch (IOException i){
            System.out.println(i);
        }finally {
            try{
                sk.close();
                running = false;
            }catch (IOException i){}
        }
    }
```
### ตัวอย่าง Code ของการเชื่อมต่อเข้าสู่ Lobby
```java
@Override
    public void actionPerformed(ActionEvent e) {
        String cmd = e.getActionCommand();
        if (cmd.equals("Connect")) {
            login.setVisible(false);

            try {
                s = new Socket(ipField.getText(), 5555);

                in = new BufferedReader(new InputStreamReader(s.getInputStream()));
                out = new PrintWriter(s.getOutputStream(), true);
                objIn = new ObjectInputStream(s.getInputStream());
                out.println("id " + user.getId());

                new Thread(new Runnable() {
                    //read thread
                    @Override
                    public void run() {
                        while (true) {

                            try {
                                dataIn = in.readLine();
                                if (dataIn.equals("start")) {

                                    System.out.println("game start");
                                    try {

                                        System.out.println("ink");
                                        quiz = (Quiz) objIn.readObject();

                                        System.out.println("recv obj");
                                        System.out.println(quiz.toString());
                                        gameplay(quiz);

                                    } catch (Exception ex) {
                                        ex.printStackTrace();
                                    }

                                }
                            } catch (IOException ex) {
                                Logger.getLogger(Student.class.getName()).log(Level.SEVERE, null, ex);
                            }

                        }
                    }
                }).start();

            } catch (IOException e1) {
                e1.printStackTrace();
                game.setVisible(false);
            }
        }
    
```



# 👥Team Member
|<a href=""><img src="https://scontent.fbkk2-8.fna.fbcdn.net/v/t1.0-9/18156901_1456506974417122_2622418456792260905_n.jpg?_nc_cat=109&_nc_ht=scontent.fbkk2-8.fna&oh=0c174e778166cbfb620e3f7eadd1ea87&oe=5C9609FB" width="200px"></a>  |<a href=""><img src="https://scontent.fbkk2-7.fna.fbcdn.net/v/t1.0-9/10806376_942596332434956_7575925399337993121_n.jpg?_nc_cat=108&_nc_ht=scontent.fbkk2-7.fna&oh=8e2b5485f40b727528854d152fdfec94&oe=5CADAD56" width="200px"></a>  |
| :-: | :-: |
|นายกวีพล ขุนศรี|นายชยากร เทียนขาว|
|60070003 |      60070013      |
|    @Supermalonz    |     @Chayakorn     |

# 👨‍🏫  Assistant Adviser
|![](https://avatars3.githubusercontent.com/u/25024858?s=150&v=4)|ผศ.ดร. ธนิศา นุ่มนนท์|
|--|--|
