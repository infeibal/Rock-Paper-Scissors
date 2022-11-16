# Rock-Paper-Scissors
It`s just a "Rock-Paper-Scissors" game

const rock = ('rock')
const paper = ('paper')
const scissors = ('scissors')
const value = ['rock', 'paper', 'scissors']
function game(user1) {
    var user2 = Math.floor(Math.random() * value.length) 
    var user2 = value[user2]
    if (user1 != rock && user1 != paper && user1 != scissors) {
        console.log('user1 is a wrong value')
        return       
    } if (user2 != rock && user2 != paper && user2 != scissors) {
        console.log('user2 is a wrong value')
        return
    } if (user1 == user2) {
        console.log(`user1: ${user1}, user2: ${user2}. Draw`)
        return
    } if (user1 == rock && user2 == paper) {
        console.log(`user1: ${user1}, user2: ${user2}. user2 Win`)
        return
    } if (user1 == rock && user2 == scissors) {
        console.log(`user1: ${user1}, user2: ${user2}. user1 Win`)
        return
    } if (user1 == paper && user2 == scissors) {
        console.log(`user1: ${user1}, user2: ${user2}. user2 win`)
        return
    } if (user1 == paper && user2 == rock) {
        console.log(`user1: ${user1}, user2: ${user2}. user1 win`)
        return
    }  if (user1 == scissors && user2 == rock) {
        console.log(`user1: ${user1}, user2: ${user2}. user2 win`)
    } if (user1 == scissors && user2 == paper) {
        console.log(`user1: ${user1}, user2: ${user2}. user1 win`)
    }
    else {
        console.log('something is wrong, you noob', user1, user2)
    }
}

game(rock) // choose ur value
