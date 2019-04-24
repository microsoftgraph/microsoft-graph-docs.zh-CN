---
title: 获取共享文件夹中的 Outlook 联系人
description: 使用 Outlook，客户可以与其他人共享文件夹，并授予对各个联系人文件夹的读取、创建、修改或删除访问权限。 通过 Outlook，客户还可以委托其他用户代表自己执行操作。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86533a28c0af206458b63fd19f32f01c5b68710b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585438"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="2769c-104">获取共享文件夹中的 Outlook 联系人</span><span class="sxs-lookup"><span data-stu-id="2769c-104">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="2769c-105">使用 Outlook，客户可以与其他人共享文件夹，并授予对各个联系人文件夹的“读取”、“创建”、“修改”或“删除”访问权限。</span><span class="sxs-lookup"><span data-stu-id="2769c-105">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="2769c-106">此外，使用 Outlook，客户还可以委托其他用户代表自己执行操作，并访问特定文件夹或客户的整个邮箱；在 Outlook 中，这也称为“委托”。</span><span class="sxs-lookup"><span data-stu-id="2769c-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="2769c-107">Microsoft Graph 以编程方式支持在其他用户共享的联系人文件夹中获取联系人，以及获取共享文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="2769c-107">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="2769c-108">此支持还适用于已委托的邮箱中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="2769c-108">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="2769c-109">例如，Garth 已与 John 共享自定义联系人文件夹并向 John 授予读取权限。</span><span class="sxs-lookup"><span data-stu-id="2769c-109">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="2769c-110">如果 John 已登录应用并提供委托的权限（Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），应用便能访问 Garth 的自定义联系人文件夹和该文件夹中的联系人，如下所述。</span><span class="sxs-lookup"><span data-stu-id="2769c-110">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

> <span data-ttu-id="2769c-111">**注意**通过共享权限（Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），你可以在共享或委托文件夹中读取或写入联系人。</span><span class="sxs-lookup"><span data-stu-id="2769c-111">**Note** The sharing permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared) allow you to read or write contacts in a shared or delegated folder.</span></span> <span data-ttu-id="2769c-112">它们不支持[订阅此类文件夹中的项的更改通知](webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="2769c-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="2769c-113">若要对租户中共享、委托或任何其他用户的联系人文件夹中的联系人设置更改通知订阅，请使用应用程序权限 Contacts.Read。</span><span class="sxs-lookup"><span data-stu-id="2769c-113">To set up change notification subscriptions on contacts in a shared, delegated, or any other user's contact folder in the tenant, use the application permission, Contacts.Read.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="2769c-114">获取共享文件夹中的联系人</span><span class="sxs-lookup"><span data-stu-id="2769c-114">Get a contact in the shared folder</span></span>

<span data-ttu-id="2769c-115">可在 Garth 已与 John 共享的自定义联系人文件夹中获取特定联系人：</span><span class="sxs-lookup"><span data-stu-id="2769c-115">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="2769c-116">成功完成后，你将收到“HTTP 200 正常”消息和由来自 Garth 共享联系人文件夹的 `{id}` 标识的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例。</span><span class="sxs-lookup"><span data-stu-id="2769c-116">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="2769c-117">获取共享文件夹中的所有联系人</span><span class="sxs-lookup"><span data-stu-id="2769c-117">Get all contacts in the shared folder</span></span>

<span data-ttu-id="2769c-118">获取 Garth 共享联系人文件夹中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="2769c-118">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="2769c-119">成功完成后，你将收到“HTTP 200 正常”消息和 Garth 共享联系人文件夹中的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例的集合。</span><span class="sxs-lookup"><span data-stu-id="2769c-119">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="2769c-120">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="2769c-120">Get the shared folder</span></span>

<span data-ttu-id="2769c-121">获取 Garth 已与 John 共享的联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="2769c-121">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="2769c-122">成功完成后，你将收到“HTTP 200 正常”消息和表示 Garth 共享联系人文件夹的 [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) 实例。</span><span class="sxs-lookup"><span data-stu-id="2769c-122">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="2769c-123">如果 Garth 已向 John 委托其整个邮箱，则将适用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="2769c-123">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="2769c-124">如果 Garth 未与 John 共享联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="2769c-124">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="2769c-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="2769c-125">Next steps</span></span>

<span data-ttu-id="2769c-126">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="2769c-126">Find out more about:</span></span>

- [<span data-ttu-id="2769c-127">为何要与 Outlook 个人联系人集成</span><span class="sxs-lookup"><span data-stu-id="2769c-127">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="2769c-128">Microsoft Graph v1.0 中的[联系人 API](/graph/api/resources/contact?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="2769c-128">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
