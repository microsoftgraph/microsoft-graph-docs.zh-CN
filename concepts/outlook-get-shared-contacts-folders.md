---
title: 获取共享文件夹中的 Outlook 联系人
description: " 另外，还有 "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091792"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="6fa5c-103">获取共享文件夹中的 Outlook 联系人</span><span class="sxs-lookup"><span data-stu-id="6fa5c-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="6fa5c-104">使用 Outlook，客户可以与其他人共享文件夹，并授予对各个联系人文件夹的“读取”、“创建”、“修改”或“删除”访问权限。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="6fa5c-105">此外，使用 Outlook，客户还可以委托其他用户代表自己执行操作，并访问特定文件夹或客户的整个邮箱；在 Outlook 中，这也称为“委托”。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="6fa5c-106">Microsoft Graph 以编程方式支持在其他用户共享的联系人文件夹中获取联系人，以及获取共享文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="6fa5c-107">此支持还适用于已委托的邮箱中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="6fa5c-108">例如，Garth 已与 John 共享自定义联系人文件夹并向 John 授予读取权限。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="6fa5c-109">如果 John 已登录应用并提供委托的权限（Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），应用便能访问 Garth 的自定义联系人文件夹和该文件夹中的联系人，如下所述。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="6fa5c-110">获取共享文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="6fa5c-110">Get a message in the shared folder</span></span>

<span data-ttu-id="6fa5c-111">可在 Garth 已与 John 共享的自定义联系人文件夹中获取特定联系人：</span><span class="sxs-lookup"><span data-stu-id="6fa5c-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="6fa5c-112">成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 共享联系人文件夹的 `{id}` 标识的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="6fa5c-113">获取共享文件夹中的所有联系人</span><span class="sxs-lookup"><span data-stu-id="6fa5c-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="6fa5c-114">获取 Garth 共享联系人文件夹中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="6fa5c-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="6fa5c-115">成功完成后，你将收到“HTTP 200 正常”消息和 Garth 共享联系人文件夹中的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="6fa5c-116">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="6fa5c-116">Get the shared folder</span></span>

<span data-ttu-id="6fa5c-117">获取 Garth 已与 John 共享的联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="6fa5c-118">成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 共享联系人文件夹的 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) 实例。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="6fa5c-119">如果 Garth 已向 John 委托其整个邮箱，则将适用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="6fa5c-120">如果 Garth 未与 John 共享联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-120">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="6fa5c-121">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6fa5c-121">Next steps</span></span>

<span data-ttu-id="6fa5c-122">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="6fa5c-122">Find out more about:</span></span>

- [<span data-ttu-id="6fa5c-123">为何要与 Outlook 个人联系人集成</span><span class="sxs-lookup"><span data-stu-id="6fa5c-123">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="6fa5c-124">Microsoft Graph v1.0 中的[联系人 API](/graph/api/resources/contact?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="6fa5c-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>