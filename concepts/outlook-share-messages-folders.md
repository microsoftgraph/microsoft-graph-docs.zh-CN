---
title: 获取共享文件夹或委托文件夹中的 Outlook 邮件
description: 使用 Outlook，客户可以与其他人共享邮件文件夹，并授予对各个文件夹的读取、创建、修改或删除访问权限。 通过 Outlook，客户还可以委托其他用户代表自己执行操作。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6de4ee7ca1ed179bc538bb7aa1f2a3dacb8adb80
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013441"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="e71a4-104">获取共享文件夹或委托文件夹中的 Outlook 邮件</span><span class="sxs-lookup"><span data-stu-id="e71a4-104">Get Outlook messages in a shared or delegated folder</span></span>

<span data-ttu-id="e71a4-105">使用 Outlook，客户可以与其他人共享邮件文件夹，并授予对各个文件夹的“读取”、“创建”、“修改”或“删除”访问权限。</span><span class="sxs-lookup"><span data-stu-id="e71a4-105">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="e71a4-106">此外，使用 Outlook，客户还可以委托其他用户代表自己执行操作，并访问特定邮件文件夹或客户的整个邮箱；在 Outlook 中，这也称为“委托”。</span><span class="sxs-lookup"><span data-stu-id="e71a4-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="e71a4-107">Microsoft Graph 以编程方式支持在其他用户共享的邮件文件夹中获取邮件，以及获取共享文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="e71a4-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="e71a4-108">此支持还适用于已委托的文件夹。</span><span class="sxs-lookup"><span data-stu-id="e71a4-108">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="e71a4-109">例如，Garth 已与 John 共享自己的收件箱，并向 John 授予对自己收件箱的读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="e71a4-109">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="e71a4-110">如果 John 已登录应用并授予委托的权限（Mail.Read.Shared 或 Mail.ReadWrite.Shared），应用便能访问 Garth 的邮件和收件箱，如下所述。</span><span class="sxs-lookup"><span data-stu-id="e71a4-110">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="e71a4-111">Microsoft Graph 权限</span><span class="sxs-lookup"><span data-stu-id="e71a4-111">Microsoft Graph permissions</span></span>

<span data-ttu-id="e71a4-112">使用委派权限，`Mail.Read.Shared` 或 `Mail.ReadWrite.Shared`，以分别在共享或委派文件夹中读取或写入邮件。</span><span class="sxs-lookup"><span data-stu-id="e71a4-112">Use the delegated permissions, `Mail.Read.Shared` or `Mail.ReadWrite.Shared`, to respectively read or write messages in a shared or delegated folder.</span></span> 

<span data-ttu-id="e71a4-113">请注意，这两种权限不支持就共享或委派文件夹中的项目 [订阅更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="e71a4-113">Note that those two permissions do not support [subscribing to change notifications](webhooks.md) on items in shared or delegated folders.</span></span> <span data-ttu-id="e71a4-114">若要对租户中共享、委派或任何其他用户邮件文件夹中的邮件设置更改通知订阅，请使用应用程序权限，`Mail.Read`。</span><span class="sxs-lookup"><span data-stu-id="e71a4-114">To set up change notification subscriptions on messages in a shared, delegated, or any other user's mail folder in the tenant, use the application permission, `Mail.Read`.</span></span>

<span data-ttu-id="e71a4-115">有关详细信息，请参阅 [邮件权限](permissions-reference.md#mail-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e71a4-115">For more information, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="e71a4-116">获取共享文件夹中的邮件</span><span class="sxs-lookup"><span data-stu-id="e71a4-116">Get a message in the shared folder</span></span>

<span data-ttu-id="e71a4-117">你可以在 Garth 的收件箱中获取特定邮件：</span><span class="sxs-lookup"><span data-stu-id="e71a4-117">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="e71a4-118">成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 收件箱的 `{id}` 标识的[消息](/graph/api/resources/message)实例。</span><span class="sxs-lookup"><span data-stu-id="e71a4-118">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="e71a4-119">获取共享文件夹中的全部邮件</span><span class="sxs-lookup"><span data-stu-id="e71a4-119">Get all messages in the shared folder</span></span>

<span data-ttu-id="e71a4-120">获取 Garth 收件箱中的所有邮件：</span><span class="sxs-lookup"><span data-stu-id="e71a4-120">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="e71a4-121">成功完成后，你将收到“HTTP 200 正常”消息和 Garth 收件箱中的[消息](/graph/api/resources/message)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="e71a4-121">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="e71a4-122">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="e71a4-122">Get the shared folder</span></span>

<span data-ttu-id="e71a4-123">获取 Garth 与 John 共享的文件夹（收件箱）。</span><span class="sxs-lookup"><span data-stu-id="e71a4-123">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="e71a4-124">成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 收件箱文件夹的 [mailFolder](/graph/api/resources/mailfolder) 实例。</span><span class="sxs-lookup"><span data-stu-id="e71a4-124">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="e71a4-125">如果 Garth 已经委派 John 进一步访问他的收件箱，或者如果 Garth 已将其整个邮箱委派给 John，那么可应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="e71a4-125">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="e71a4-126">如果 Garth 既未与 John 共享自己的收件箱，也未将自己的邮箱委托给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称便会返回错误。</span><span class="sxs-lookup"><span data-stu-id="e71a4-126">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="e71a4-127">后续步骤</span><span class="sxs-lookup"><span data-stu-id="e71a4-127">Next steps</span></span>

<span data-ttu-id="e71a4-128">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="e71a4-128">Find out more about:</span></span>

- [<span data-ttu-id="e71a4-129">为什么与 Outlook 邮件集成</span><span class="sxs-lookup"><span data-stu-id="e71a4-129">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="e71a4-130">[使用邮件 API](/graph/api/resources/mail-api-overview) 及其在 Microsoft Graph v1.0 中的[用例](/graph/api/resources/mail-api-overview#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="e71a4-130">[Using the mail API](/graph/api/resources/mail-api-overview) and its [use cases](/graph/api/resources/mail-api-overview#common-use-cases) in Microsoft Graph v1.0.</span></span>
