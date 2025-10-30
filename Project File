
using System;
using System.Runtime.Remoting.Lifetime;
namespace ProjectFile
{
    class Program
    {
        static void Main(string[] args)
        {
            //init variables
            int userGuess;
            Random rnd = new Random();//Camryn Creating a random string
            int rndNumber = rnd.Next(1, 100);//Camryn Setting the random string to be between 1 and 100
            int attempts = 0;

            //Run until user guesses correctly
            while (true)
            {
                Console.WriteLine("Please enter a number between 1 and 100: "); //(Mitchell) Prompt user for input
                string userInput = Console.ReadLine();//read user input (Mitchell)
                attempts++; //track attempts (Mitchell)
                while (!int.TryParse(userInput, out userGuess)) // Validate input and turn string to int(Mitchell)
                {
                    Console.WriteLine("Invalid input. Please try entering a valid number.");
                    userInput = Console.ReadLine().Trim();
                    attempts++;
                }//  (Mitchell)

                if (userGuess > rndNumber) //Ronald - Check if guess is too high
                {
                    Console.WriteLine("Your guess is too high!");
                }
                else if (userGuess < rndNumber) //Check if guess if too low
                { //Mateo
                    Console.WriteLine("Your guess is too low. Guess Higher");
                }

                else if (userGuess == rndNumber && attempts == 1) { //Caleb only one attempts
                    Console.WriteLine(" Congrats you got it right, and in one guess. Wow your either super lucky, or did you possibly cheat. ");
                    break;
                }
                else if (userGuess == rndNumber && attempts == 2) { //Caleb 2 attempts
                    Console.WriteLine(" Congrats you got it right. You only did it in two guesses.Not as good as one, but still great ");
                    break;
                }
                else if (userGuess == rndNumber && attempts == 3) { //Caleb 3 attempts
                    Console.WriteLine(" Three guesses is still lucky. Especially with how many numbers you had to guess from. ");
                    break;
                }
                else if (userGuess == rndNumber && attempts == 4) { //Caleb 4 attempts
                    Console.WriteLine(" Oh four guesses you must of really been racking your brain for that one ");
                    break;
                }
                else if (userGuess == rndNumber && attempts == 5) {//Caleb 5 attempts
                    Console.WriteLine(" Five guesses you really are just passing this game. Better luck next time. ");
                    break;
                }
                else if (userGuess == rndNumber && attempts > 5) {//Camryn If more then 5 message
                    Console.WriteLine("Wow if I'm being honest you kinda suck at this or are REALLY unlucky :("); //Camryn Message for attempts above 5
                    break;
                }
            }
        }
    }
}
