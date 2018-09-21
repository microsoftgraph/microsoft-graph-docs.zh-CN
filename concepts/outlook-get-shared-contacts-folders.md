# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="92536-101">获取共享文件夹中的 Outlook 联系人</span><span class="sxs-lookup"><span data-stu-id="92536-101">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="92536-102">Outlook 允许客户相互共享文件夹，并提供对个人联系人文件夹的“读取”、“创建”、“修改”或“删除”等访问权限。</span><span class="sxs-lookup"><span data-stu-id="92536-102">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="92536-103">Outlook 还允许客户委派另一个用户代表客户操作并访问特定的文件夹或客户的整个邮箱；这在 Outlook 中也称为“委派”。</span><span class="sxs-lookup"><span data-stu-id="92536-103">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="92536-104">Microsoft Graph 以编程方式支持在其他用户共享的联系人文件夹中获取联系人，以及获取共享文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="92536-104">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="92536-105">该支持还适用于委派邮箱中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="92536-105">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="92536-106">例如，Garth 与 John 共享了他的自定义联系人文件夹，并授予 John 读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="92536-106">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="92536-107">如果 John 已登录你的应用并提供了委派权限 (Contacts.Read.Shared or Contacts.ReadWrite.Shared)，则你的应用将能够访问 Garth 的自定义联系人文件夹和文件夹中的联系人，如下所述。</span><span class="sxs-lookup"><span data-stu-id="92536-107">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="92536-108">获取共享文件夹中联系人</span><span class="sxs-lookup"><span data-stu-id="92536-108">Get a message in the shared folder</span></span>

<span data-ttu-id="92536-109">你可以获取 Garth 与 John 共享的自定义联系人文件夹中的特定联系人：</span><span class="sxs-lookup"><span data-stu-id="92536-109">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="92536-110">成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 共享联系人文件夹中由 `{id}` 标识的[联系人](../api-reference/v1.0/resources/contact.md)实例。</span><span class="sxs-lookup"><span data-stu-id="92536-110">On successful completion, you'll get HTTP 200 OK and the [message](../api-reference/v1.0/resources/contact.md) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="92536-111">获取共享文件夹中的所有联系人</span><span class="sxs-lookup"><span data-stu-id="92536-111">Get all messages in the shared folder</span></span>

<span data-ttu-id="92536-112">获取 Garth 的共享联系人文件夹中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="92536-112">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="92536-113">成功完成后，你将收到“HTTP 200 正常”消息以及 Garth 共享联系人文件夹中的[联系人](../api-reference/v1.0/resources/contact.md)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="92536-113">On successful completion, you'll get HTTP 200 OK and a collection of [message](../api-reference/v1.0/resources/contact.md) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="92536-114">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="92536-114">Get the shared folder</span></span>

<span data-ttu-id="92536-115">获取 Garth 与 John 共享的联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="92536-115">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="92536-116">成功完成后，你将收到“HTTP 200 正常”消息以及表示 Garth 共享联系人文件夹的 [contactFolder](../api-reference/v1.0/resources/contactfolder.md) 实例。</span><span class="sxs-lookup"><span data-stu-id="92536-116">On successful completion, you'll get HTTP 200 OK and a [mailFolder](../api-reference/v1.0/resources/contactfolder.md) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="92536-117">如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="92536-117">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="92536-118">如果 Garth 未与 John 共享联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="92536-118">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="92536-119">后续步骤</span><span class="sxs-lookup"><span data-stu-id="92536-119">Next steps</span></span>

<span data-ttu-id="92536-120">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="92536-120">Find out more about:</span></span>

- [<span data-ttu-id="92536-121">为何要与 Outlook 个人联系人集成</span><span class="sxs-lookup"><span data-stu-id="92536-121">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="92536-122">Microsoft Graph v1.0 中的 [联系人 API](../api-reference/v1.0/resources/contact.md)。</span><span class="sxs-lookup"><span data-stu-id="92536-122">The [contacts API](../api-reference/v1.0/resources/contact.md) in Microsoft Graph v1.0.</span></span>