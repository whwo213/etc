<%@ page import="java.io.*" %>

          <%
            String sDir      = "";
            String sFileName = "";
            String sFilePath = "";
            String sLine     = "";
            String sText     = "";
            try {
              sDir      = request.getSession().getServletContext().getRealPath("/")+"WEB-INF/page/board/skin/SKIN_0000085/"+"";                                                                // 디렉토리명
              sFileName = "list.jsp";                                                   // 파일명
              sFilePath = sDir + sFileName;                                        // 파일경로

              try{
               /* File f = new File(sFilePath); // 파일객체생성
                f.createNewFile(); //파일생성
                // 파일쓰기
                FileWriter fw = new FileWriter(sFilePath); //파일쓰기객체생성
                String data = "파일에다 아무거나 적습니다.\n이거는 두번째 줄인데 아무거나 적습니다";
                fw.write(data); //파일에다 작성
                fw.close(); //파일핸들 닫기*/

                // 파일읽기
                FileReader fr = new FileReader(sFilePath); //파일읽기객체생성
//                BufferedReader br = new BufferedReader(fr); //버퍼리더객체생성
                BufferedReader br = new BufferedReader(new InputStreamReader(new FileInputStream(sFilePath),"UTF-8"));
                String line = null;
                while((line=br.readLine())!=null){ //라인단위 읽기
                  out.println(line + "<br>");
                }
              }catch (IOException e) {
                out.println(e.toString()); //에러 발생시 메시지 출력
              }

            }catch(Exception e){
              e.printStackTrace();
            }
          %>
