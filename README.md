# prompt_Engineering_1_project

**Main Goal is to how to give prompt by using Google Generative AI**

**Main Points : In a Good Prompt**

1. Content               - What You Want to do
2. Role                  - Assign Role to AI Assitant
3. Constrains            - How many words,length, is a Conditions of a prompt
4. Instructions          - using this to implement the rules
5. Examples              - Examples of the content
6. Chain of thoughts     - what in your mind Exactly that can be write


        importing the GenAI Models by using Google generative AI.
        
          >> import google.generativeai as genai


        import userdata Key is Inbulit in Google Colab It self.
        and we use this to secret key of API_Key

          >> from google.colab import userdata
          >> api_key=userdata.get('GOOGLE_API_KEY_1')

        Take a genai Model to Implement the Prompt.
        Iam taking "gemini-2.5-flash"
        you can take any model to implement the Prompt.

          >> model=genai.GenerativeModel('gemini-2.5-flash')

       What i Given in First That can be implemented by using prompt_template it means a prompt board

       Content,Role,Constrains,Instructions,Examples,Chain of Thoughts

          prompt_template = """
          
          
   **Content**           : Prepare a time table for railways compitative Exams
          
   **Role**              : Your are A mentor
          
   **Constrains**        :
                                    
                             - Explain in detail of a every subject.
                              
                             - Easy to Understand any body.
                                    
                             - Clearly mention every Point.
          
   **Instructions**      :
          
                             - Give Relavent answer by using Input.
                                    
                             - mention every subject what using in railway compitative exams.
                                    
                             - Maintain a good order time table for railway compitative exams.
                                    
                             - avoid unnessary explanation.
                                    
   **Examples**          :

                             - It can be implemted in a Daily Routine process.
                                      
   **Chain of Thoughts** :
                             - You Think like a Human Being like a mentor.
                                      
                             - you Think like a Ai Assistant Mentor.
            
            
            
   **Input**           : Prepare a time table for railways compitative Exams for a student
            
   **Output**          :
   """
          
          
   **response = model.generate_content(prompt_template)**
   **print(response)**
