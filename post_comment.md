
<code>
from beem import Hive
from beem.comment import Comment

# Define your Hive node and account credentials
node = 'https://api.hive.blog'  # Replace with your preferred Hive node
account_name = ''  # Replace with your Hive account name
posting_key = ''  # Replace with your Hive account's posting key

# Connect to the Hive blockchain
hive = Hive(node=node, keys=[posting_key])

# Set the post author and permlink where you want to comment
author = 'tin.aung.soe'  # Replace with the author of the post
permlink = 'in-winter-evening-opening-new'  # Replace with the permlink of the post

# Text of the comment
comment_text = "Your comment text here."

# Create a Comment object with the parent post details
parent_post = Comment(f'@{author}/{permlink}', blockchain_instance=hive)

# Submit the comment using the reply method
parent_post.reply(body=comment_text, author=account_name)

print("Comment submitted successfully!")

</code>
