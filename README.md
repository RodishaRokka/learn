import random

while True:
    choices = ["rock","paper","scissor"]

    computer = random.choice(choices)
    player = None

    while player not in choices:
        player = input("rock,paper or scissor?: ").lower()

    if player == computer:
        print("computer: ", computer)
        print("player: ", player)
        print("tie!")

    elif player == "rock":
        if computer == "paper":
            print("computer: ", computer)
            print("player: ", player)
            print("you loose")
        if computer == "scissor":
            print("computer: ", computer)
            print("player", player)
            print("you win")

        elif player == "paper":
            if computer == "rock":
                print("computer: ", computer)
                print("player: ", player)
                print("you win")
            if computer == "scissor":
                print("computer: ", computer)
                print("player: ", player)
                print("you loose")

        elif player == "scissor":
            if computer == "paper":
                print("computer: ", computer)
                print("player: ", player)
                print("you win")
            if computer == "rock":
                print("computer: ", computer)
                print("player: ", player)
                print("you loose")


    play_again=input("play again?(yes/no): ").lower()
    if play_again !="yes":
        break
