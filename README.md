Chess Rice Grain Puzzle:

There was once a king in India who was a big chess enthusiast and had the habit of challenging wise visitors to a game of chess. One day a traveling sage was challenged by the
king. The sage having played this game all his life all the time with people all over the world gladly accepted the Kings challenge. To motivate his opponent the king 
offered any reward that the sage could name. The sage modestly asked just for a few grains of rice in the following manner: the king was to put a single grain of rice on the 
first chess square and double it on every consequent one. The king accepted the sage’s request. Having lost the game and being a man of his word the king ordered a bag of rice
to be brought to the chessboard. Then he started placing rice grains according to the arrangement: 1 grain on the first square, 2 on the second, 4 on the third, 8 on the fourth, 
and so on. Write a python one-line program to get the total sum of rice grains king is supposed to pay sage?

##Code###

num=int(input())
if num<0:
  print("error")
elif num<=64:
  temp=1
  sum=0
  for i in range(1,num+1):
    temp=(2**i/2)
    sum=sum+temp   
  print("The Total sum of the Rice Grains king is supposed to pay sage : {} ".format(sum))
