---
title: 获取共享文件夹或委托文件夹中的 Outlook 邮件
description: 这些主题还有类似的部分：列出事件、获取事件、获取日历、列出联系人、获取联系人、获取联系人文件夹。
author: angelgolfer-ms
ms.openlocfilehash: d90fa5d37fd7a07e4069bd5bcc0eb46f0cae29a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320109"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="66f8f-103">获取共享文件夹或委托文件夹中的 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="66f8f-103">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="66f8f-104">使用 Outlook，客户可以与其他人共享邮件文件夹，并授予对各个文件夹的“读取”、“创建”、“修改”或“删除”访问权限。</span><span class="sxs-lookup"><span data-stu-id="66f8f-104">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="66f8f-105">此外，使用 Outlook，客户还可以委托其他用户代表自己执行操作，并访问特定邮件文件夹或客户的整个邮箱；在 Outlook 中，这也称为“委托”。</span><span class="sxs-lookup"><span data-stu-id="66f8f-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="66f8f-106">Microsoft Graph 以编程方式支持在其他用户共享的邮件文件夹中获取邮件，以及获取共享文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="66f8f-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="66f8f-107">此支持还适用于已委托的文件夹。</span><span class="sxs-lookup"><span data-stu-id="66f8f-107">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="66f8f-108">例如，Garth 已与 John 共享自己的收件箱，并向 John 授予对自己收件箱的读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="66f8f-108">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="66f8f-109">如果 John 已登录应用并授予委托的权限（Mail.Read.Shared 或 Mail.ReadWrite.Shared），应用便能访问 Garth 的邮件和收件箱，如下所述。</span><span class="sxs-lookup"><span data-stu-id="66f8f-109">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="66f8f-110">获取共享文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="66f8f-110">Get a message in the shared folder</span></span>

<span data-ttu-id="66f8f-111">你可以在 Garth 的收件箱中获取特定邮件：</span><span class="sxs-lookup"><span data-stu-id="66f8f-111">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="66f8f-112">成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 收件箱的 `{id}` 标识的[消息](/graph/api/resources/message?view=graph-rest-1.0)实例。</span><span class="sxs-lookup"><span data-stu-id="66f8f-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="66f8f-113">获取共享文件夹中的全部邮件</span><span class="sxs-lookup"><span data-stu-id="66f8f-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="66f8f-114">获取 Garth 收件箱中的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="66f8f-114">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="66f8f-115">成功完成后，你将收到“HTTP 200 正常”消息和 Garth 收件箱中的[消息](/graph/api/resources/message?view=graph-rest-1.0)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="66f8f-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="66f8f-116">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="66f8f-116">Get the shared folder</span></span>

<span data-ttu-id="66f8f-117">获取 Garth 与 John 共享的文件夹（收件箱）。</span><span class="sxs-lookup"><span data-stu-id="66f8f-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="66f8f-118">成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 收件箱文件夹的 [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) 实例。</span><span class="sxs-lookup"><span data-stu-id="66f8f-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="66f8f-119">如果 Garth 已经委派 John 进一步访问他的收件箱，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="66f8f-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="66f8f-120">如果 Garth 既未与 John 共享自己的收件箱，也未将自己的邮箱委托给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称便会返回错误。</span><span class="sxs-lookup"><span data-stu-id="66f8f-120">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="66f8f-121">后续步骤</span><span class="sxs-lookup"><span data-stu-id="66f8f-121">Next steps</span></span>

<span data-ttu-id="66f8f-122">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="66f8f-122">Find out more about:</span></span>

- [<span data-ttu-id="66f8f-123">为什么与 Outlook 邮件集成</span><span class="sxs-lookup"><span data-stu-id="66f8f-123">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="66f8f-124">[使用邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 及其在 Microsoft Graph v1.0 中的[用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="66f8f-124">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>