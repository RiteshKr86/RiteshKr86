while true; do
    read -p "How many files are in the current directory? " guess

    if [[ $guess -eq $num_files ]]; then
        echo "Congratulations! You guessed it correctly."
        break
    elif [[ $guess -lt $num_files ]]; then
        echo "Too low. Try again."
    else
        echo "Too high. Try again."
    fi
done
