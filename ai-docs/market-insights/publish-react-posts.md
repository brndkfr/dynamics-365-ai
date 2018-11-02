---
title: "Publish and react to posts in Market Insights | Microsoft Docs"
description: "Learn how you can react to posts or publish a new post in Market Insights."
keywords: "publish, post, like, favorite, share, private message, Market Insights"
ms.date: 10/31/2018
ms.service: dynamics-365-ai
ms.topic: article
ms.assetid: 39e71aaa-d804-4e73-b789-df185fcb7ef1
author: m-hartmann
ms.author: mhart
manager: shellyha
ms.custom: dyn365-ai-marketinsights
search.audienceType: 
  - admin
  - customizer
  - enduser
search.app: 
  - D365CE
  - D365SE
---

# Publish and react to posts

[This topic is pre-release documentation and is subject to change.]

Staying in touch with customers, prospects, and other stakeholders through social media channels is a key factor in business success. Take action on posts that you find with [!INCLUDE[Dynamics 365 AI for Market Insights](../includes/pn-market-insights-long.md)]. Share, like, or comment on [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] posts, or retweet, like, or reply to [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] posts to stay in touch with and engage with your audience. Start a conversation by writing new posts from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

<a name="Prerequisites"></a>   
## Prerequisites  
 Before you start to engage with your audience, make sure you meet the following prerequisites:  

1. You have an [Interaction user role of Responder or Manager](user-roles.md), which allows you to publicly post on social networks from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].

2. You own at least one [social profile](manage-social-profiles.md) or have it shared with you for the social networks that you want to interact on.

3. Social data is already available in your [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] solution. You can find it in the **Posts** area in **Analytics**, or through [streams](engage-on-social-networks.md)  in the **Social Center**. 

   > [!TIP]
   >  If you don’t own any social profiles, [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] posts provide the option to use [Web Intents](https://dev.twitter.com/web/intents). You must sign in to [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] to post with your profile.  

<a name="engageOverview"></a>   
## Engage on a post in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]  
[!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you proactively engage on social media or react to social data that you gather. In no time, you can compose a post, answer questions, share information, or socialize with your audience on social networks.  

The following table shows what [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you do depending on where you want to interact.  


|                                                                  |                                                                     Twitter                                                                      |                                                                                          Facebook                                                                                           |
|------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Let users know you appreciate a post they wrote](#favoriteLike) |    Like<br /><br /> ![like button on twitter in market insights](media/twitter-like-icon.png "Like button on Twitter in Market Insights")    | Like as [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] page <br /><br /> ![facebook like button in market insights](media/like-icon.png "Facebook like button in Market Insights") |
|         [Share a post with your audience](#retweetShare)         |          Retweet<br /><br /> ![retweet button in market insights](media/share-retweet-icon.png "Retweet button in Market Insights")          |                       Share<br /><br /> ![facebook share button in market insights](media/share-on-facebook-icon.png "Facebook share button in Market Insights")                        |
|             [Reply to a conversation](#commentReply)             |         Reply<br /><br /> ![twitter reply button in market insights](media/reply-icon.png "Twitter reply button in Market Insights")         |                     Comment<br /><br /> ![facebook comment button in market insights](media/facebook-comment-icon.png "Facebook comment button in Market Insights")                     |
|             [Engage in private conversations](#DMs)              | Send direct message<br /><br /> ![send message button in market insights](media/enevelope-icon.png "Send message button in Market Insights") |                      Send private message<br /><br /> ![send message button in market insights](media/enevelope-icon.png "Send message button in Market Insights")                      |
|             [Post a link to another post](#PostLink)             |   Post link<br /><br /> ![post a link button in market insights](media/post-link-action-icon.png "Post a link button in Market Insights")    |                         Post link<br /><br /> ![post a link button in market insights](media/post-link-action-icon.png "Post a link button in Market Insights")                         |
|             [Start a new conversation](#PublishPost)             |                                                                     Publish                                                                      |                                                                                           Publish                                                                                           |

> [!NOTE]
>  If you apply several actions on posts in the same post list, the system  queues all planned actions so that you can seamlessly proceed with your work. If a queued action fails, you’ll get notified directly in the application. If you switch to a different area in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] while some actions are still in the queue, the application warns you before interrupting the actions.  
> 
>  Posts that you send from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] are not picked up automatically by your search topics. Create a [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] rule to [track all tweets](add-rules-search-topic.md) from a specific author (in this case your social profile), or a [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] page rule to [capture all posts](add-rules-search-topic.md) from a specific [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] page. 

<a name="favoriteLike"></a>   
### Let users know you appreciate a post they wrote  
 When you find a post in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] that you appreciate, show its author your support and like it. You can easily do this directly from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

#### Like a post  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select the post you want to interact with.  

3. At the bottom of the post, select **Like**.
   > [!NOTE]
   > On [!INCLUDE[tn_facebook](../includes/tn-facebook.md)], you can only like posts with a [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] page profile.

4. Select the check box for the social profile that you want to like this post with.  

5. Select **Confirm**.  

<a name="retweetShare"></a>   
### Share a post with your audience  
 Some posts you find may be relevant to your audience, too. To spread the word, retweet or share them with a few selects directly from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

#### Retweet or share a post  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select the post you want to interact with.  

3. At the bottom of the post, select **Retweet** ![retweet button in market insights](media/share-retweet-icon.png "Retweet button in Market Insights") or **Share** ![facebook share button in market insights](media/share-on-facebook-icon.png "Facebook share button in Market Insights").  

   > [!NOTE]
   >  You can retweet posts only from public [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] profiles. If a [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] profile is protected, you might still be able to read its posts if you’re a confirmed follower, but you won’t be able to retweet.  

4. Select the check box for the  social profile that you want to share this post with.  

5. Type your message in the text field.  

6. Select **Retweet** ![retweet button in market insights](media/share-retweet-icon.png "Retweet button in Market Insights") or **Share** ![facebook share button in market insights](media/share-on-facebook-icon.png "Facebook share button in Market Insights").  

<a name="commentReply"></a>   
### Reply to a conversation  
 Reply to questions, requests, and feedback on [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] and on [!INCLUDE[tn_facebook](../includes/tn-facebook.md)] pages directly from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

 Conversations on [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] usually start with public posts. Especially with support requests, additional information is often required (for example, a billing number or a real name confirmation). This additional information usually isn’t intended for the public and needs to be shared in a private way. [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you add a link to start a private conversation to any public reply on [!INCLUDE[tn_twitter](../includes/tn-twitter.md)]. This lets you turn any public conversation into a private one, without losing the context.  

#### Comment or reply to a post  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select the post you want to interact with.  

3. At the bottom of the post, select **Comment** ![facebook comment button in market insights](media/facebook-comment-icon.png "Facebook comment button in Market Insights") or **Reply** ![twitter reply button in market insights](media/reply-icon.png "Twitter reply button in Market Insights") .  

4. In the header of the text box, select the social profile that you want to post with.  

5. Type your message in the text box.  

6. Optionally, you can add a photo to the reply.  

    Photos need to be in .png, .jpg, or .gif format. Maximum file sizes apply, depending on which social network you want to post to.  

7. To publish the message on behalf of the selected social profile, select **Comment** ![facebook comment button in market insights](media/facebook-comment-icon.png "Facebook comment button in Market Insights") or **Reply** ![twitter reply button in market insights](media/reply-icon.png "Twitter reply button in Market Insights") .  

    You'll see a star symbol added to the Comment/Reply symbol (![facebook comment button in market insights](media/facebook-comment-icon.png "Facebook comment button in Market Insights")) if another user has already replied to this post from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

#### Add a link to send a private message from a public conversation on Twitter  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select the [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] post that you want to interact with.  

3. At the bottom of the post, select **Reply** ![twitter reply button in market insights](media/reply-icon.png "Twitter reply button in Market Insights") .  

4. In the header of the text  field, select the social profile that you want to post with.  

5. Type your message in the text  field.  

6. Select the **Add “Send a private message” link** check box.  

    A link to reply to this conversation in a private message is added to your reply.  

7. To publish the message on behalf of the selected social profile, select **Reply** ![twitter reply button in market insights](media/reply-icon.png "Twitter reply button in Market Insights") .  

To learn more about how [!INCLUDE[tn_twitter](../includes/tn-twitter.md)] guides users from public to private conversations, see [Twitter Help: Public to private conversation](https://business.twitter.com/help/public-to-private-conversation).  

<a name="PostLink"></a>   
### Post a link to another post  
Share a link to a public post along with your own comments as a new post directly from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

#### Create a new post with a link to a post found in [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select the post you want to interact with.  

3. At the bottom of the post, select the **Post Link** button ![post a link button in market insights](media/post-link-action-icon.png "Post a link button in Market Insights").  

4. Select the check box for the social profile that you want to send this post with.  

   > [!NOTE]
   > When you share to [!INCLUDE[pn-linkedin](../includes/pn-linkedin.md)], you can choose between two visibility options: Either share the post with everyone on [!INCLUDE[pn-linkedin](../includes/pn-linkedin.md)] or only with your network.
   > 
   > You can't share the URL of a [!INCLUDE[tn-facebook](../includes/tn-facebook.md)] comment on [!INCLUDE[tn-facebook](../includes/tn-facebook.md)], and we'll hide the social profiles for [!INCLUDE[tn-facebook](../includes/tn-facebook.md)] when you try to post a link to a [!INCLUDE[tn-facebook](../includes/tn-facebook.md)] comment.  

5. Optionally, type additional text in the text field.  

6. Select **Post**.  

<a name="PublishPost"></a>   
### Start a new conversation  
 Start the conversation with your audience and publish new posts directly from within [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)].  

 You must have at least one [owned or shared social profile](manage-social-profiles.md) to see the **Publish** button.  

#### Compose a new post in Social Center  

1. Go to **Social Center**.  

2. To show the compose form, select **Publish**.  

   > [!TIP]
   >  If you want to publish the same content with a different social profile, in the **Publish** pane, select **Include the content from the previous post**. This prepares the same post for your convenience so you can easily edit it for your targeted audience.  

3. Select the message type for this post.  

4. Select the check box for the  social profile that you want to send this post with.  

5. In the text entry field, type the text for the post.  

6. Optionally, you can add a photo to the post.  

    Photos need to be in .png, .jpg, or .gif format. Maximum file sizes apply, depending on which social network you want to post to. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Add media to posts](publish-react-posts.md#addMedia)  

7. To publish the post on the corresponding social network, select **Send**.  

<a name="DMs"></a>   
### Engage in private conversations  
 Quickly respond to a private conversation through one of your social profiles directly from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]. You can allow the data acquisition of your private messages so that other users of your organization’s solution can see the full context of the conversations.  

 If data acquisition for private conversation from a social profile is allowed, and a search topic contains a Private Messages rule for the same social profile, all direct messages, including attachments, are visible to other users of the same [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] solution. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [Data retention in Market Insights](data-retention.md)  

<a name="dmTwitter"></a>   
#### Send a direct message on Twitter from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select a direct message that your search topics found.  

3. At the bottom of the post, select **Direct Message**.  

   > [!IMPORTANT]
   >  You can reply to a direct message only with the social profile that received the message. [!INCLUDE[proc_more_information](../includes/proc-more-information.md)] [About Direct Messages](https://support.twitter.com/articles/14606-about-direct-messages)  

4. Type your message in the text field. [!INCLUDE[Dynamics 365 AI for Market Insights](../includes/pn-market-insights-long.md)] limits direct  messages to 10,000 characters. When you get close to the character limit, [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] will show a counter so you can see if you need to revise your message to fit within the maximum character limit.  

5. To post on behalf of the selected social profile, select **Send Direct Message**.  

<a name="dmFacebook"></a>   
#### Send a direct message on Facebook from [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)]  

1. Go to **Social Center**.  

    --OR--  

    When you're working in Analytics pages, select **Posts**.  

2. Select a private message that your search topics found.  

3. At the bottom of the post, select **Private Message**.  

   > [!NOTE]
   >  When you reply to a private message, you can reply to a single recipient only with the social profile that received the private message. Group conversations aren’t supported in private messages.  

4. Type your message in the text entry field. [!INCLUDE[Dynamics 365 AI for Market Insights](../includes/pn-market-insights-long.md)] limits direct  messages to 10,000 characters. When you get close to the character limit, [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] will show a counter so you can optimize the length of your content.  

5. Select **Send Private Message** to post on behalf of the selected social profile.  

<a name="addMedia"></a>   
### Add media to posts  
 [!INCLUDE[Market Insights](../includes/pn-market-insights-short.md)] lets you add a single photo to posts while publishing from within the application.  

 Supported file types: .png, .jpg, .gif  

 Depending on the social network that media is posted to, different limitations in file sizes apply.  

 Read more about the [maximum file size on Twitter](https://dev.twitter.com/rest/public/uploading-media).  

 Read more about the [maximum file size on Facebook](https://www.facebook.com/help/167931376599294).  

> [!NOTE]
>  When you use a large file, it can take a long time to upload. Also, timeouts can happen when the upload takes too long due to limited bandwidth.  If this happens, try resizing the image to reduce the file size, or try again with more bandwidth.  

### See Also  
 [Engage on social networks](engage-on-social-networks.md)   
 [Work with posts](work-with-posts.md)   
 [Manage social profiles](manage-social-profiles.md)