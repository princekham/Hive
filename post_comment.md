# from https://peakd.com/hive-169321/@steevc/writing-a-hive-bot-with-beem

from datetime import datetime, timedelta, date
from beem import Hive
from beem.account import Account
from beem.amount import Amount
from beem.blockchain import Blockchain
from beem.comment import Comment
from beem.exceptions import ContentDoesNotExistsException
from beem.instance import set_shared_blockchain_instance
import random

hive = Hive(node=['https://api.hive.blog'], keys={'posting':posting})
set_shared_blockchain_instance(hive)
chain = Blockchain()

# This is comment text I think.

def addComment(comm):
  #  image = random.choice(gifs) # This one no need
    text = f'''Here is your Proof of Brian. I think you meant #ProofOfBrain
![Brian]({image["Pic"]})
[Source]({image["Source"]})'''
    comm.reply(body=text,author=postacc)  #this one is for replying to a post
    #return text

            author = post['author']  #here author should be princekham
            c = Comment(post)      # post should be the post I am going to comment
            addComment(c)

            
