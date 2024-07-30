def get_questions():
    return [
        {
            "question": "What is the capital of France?",
            "options": ["A) Paris", "B) London", "C) Berlin", "D) Madrid"],
            "answer": "A"
        },
        {
            "question": "What is 2 + 2?",
            "options": ["A) 3", "B) 4", "C) 5", "D) 6"],
            "answer": "B"
        },
        {
            "question": "Who wrote 'To Kill a Mockingbird'?",
            "options": ["A) Harper Lee", "B) Mark Twain", "C) J.K. Rowling", "D) Ernest Hemingway"],
            "answer": "A"
        }
    ]

def ask_question(question_data):
    print(question_data["question"])
    for option in question_data["options"]:
        print(option)
    
    answer = input("Enter your answer (A, B, C, D): ").upper()
    while answer not in ['A', 'B', 'C', 'D']:
        answer = input("Invalid input. Please enter A, B, C, or D: ").upper()
    
    return answer

def main():
    questions = get_questions()
    score = 0
    
    for question_data in questions:
        user_answer = ask_question(question_data)
        if user_answer == question_data["answer"]:
            print("Correct!")
            score += 1
        else:
            print(f"Incorrect! The correct answer is {question_data['answer']}")
        print()
    
    print(f"Your final score is: {score}/{len(questions)}")

if __name__ == "__main__":
    main()
