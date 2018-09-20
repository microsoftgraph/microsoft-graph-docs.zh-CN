# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="bcfd8-101">获取一个共享或委派文件夹中的 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="bcfd8-101">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="bcfd8-102">Outlook 允许客户相互共享邮件文件夹，并提供对个人文件夹的“读取”、“创建”、“修改”或“删除”等访问权限。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="bcfd8-103">Outlook 还允许客户委派另一个用户代表客户操作并访问特定的邮件文件夹或客户的整个邮箱；这在 Outlook 中也称为“委派”。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="bcfd8-104">Microsoft Graph 以编程方式支持在其他用户共享的邮件文件夹中获取邮件，以及获取共享文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="bcfd8-105">该支持还适用于已委派的文件夹。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-105">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="bcfd8-106">举个例子，Garth 已经与 John 共享并授予他 Garth 收件箱的读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-106">As an example, Garth has shared with John read access to Garth's Inbox.</span></span> <span data-ttu-id="bcfd8-107">如果 John 已登录你的应用并提供了委派权限 (Mail.Read.Shared or Mail.ReadWrite.Shared)，则你的应用将能够访问 Garth 的邮件和 Garth 的收件箱，如下所述。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="bcfd8-108">获取共享文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="bcfd8-108">Get a message in the shared folder</span></span>

<span data-ttu-id="bcfd8-109">你可以在 Garth 的收件箱中获取特定邮件：</span><span class="sxs-lookup"><span data-stu-id="bcfd8-109">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="bcfd8-110">成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 收件箱的 `{id}` 标识的[消息](../api-reference/v1.0/resources/message.md)实例。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/message.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="bcfd8-111">获取共享文件夹中的全部邮件</span><span class="sxs-lookup"><span data-stu-id="bcfd8-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="bcfd8-112">获取 Garth 收件箱中的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="bcfd8-112">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="bcfd8-113">成功完成后，你将收到“HTTP 200 正常”消息和 Garth 收件箱中的[消息](../api-reference/v1.0/resources/message.md)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/message.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="bcfd8-114">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="bcfd8-114">Get the shared folder</span></span>

<span data-ttu-id="bcfd8-115">获取 Garth 与 John 共享的文件夹（收件箱）。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="bcfd8-116">成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 收件箱文件夹的 [mailFolder](../api-reference/v1.0/resources/mailfolder.md) 实例。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/mailfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="bcfd8-117">如果 Garth 已经委派 John 进一步访问他的收件箱，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="bcfd8-118">如果 Garth 未与 John 共享他的收件箱，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-118">If Garth has not shared his message folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="bcfd8-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="bcfd8-119">Next steps</span></span>

<span data-ttu-id="bcfd8-120">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="bcfd8-120">Find out more about:</span></span>

- [<span data-ttu-id="bcfd8-121">为什么与 Outlook 邮件集成</span><span class="sxs-lookup"><span data-stu-id="bcfd8-121">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="bcfd8-122">[使用邮件 API](../api-reference/v1.0/resources/mail_api_overview.md) 及其在 Microsoft Graph v1.0 中的[用例](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="bcfd8-122">[Using the mail API](../api-reference/v1.0/resources/mail_api_overview.md) and its [use cases](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases) in Microsoft Graph v1.0.</span></span>