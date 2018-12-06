---
title: 获取一个共享文件夹中的 Outlook 联系人
description: " 这也是 "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091792"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="6f7c5-103">获取一个共享文件夹中的 Outlook 联系人</span><span class="sxs-lookup"><span data-stu-id="6f7c5-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="6f7c5-104">Outlook 允许客户与另一个共享文件夹，并提供"的读取"、"创建"、"修改"删除"的各个联系人文件夹的访问。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-104">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="6f7c5-105">Outlook 还允许委派另一个用户操作代表客户，和访问特定的文件夹或客户的整个邮箱; 客户这也称为是在 Outlook 中的"委派"。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="6f7c5-106">以编程方式，Microsoft Graph 支持具有已由其他用户共享的联系人文件夹中获取联系人，以及获取共享的文件夹本身。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-106">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="6f7c5-107">支持也适用于委派邮箱中的文件夹。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="6f7c5-108">例如，Garth 具有共享 John 自定义联系人文件夹，并且授予 John 读取访问权限。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="6f7c5-109">如果 John 已登录到您的应用程序，并提供委派的权限 （Contacts.Read.Shared 或 Contacts.ReadWrite.Shared），您的应用程序都将能够访问 Garth 的自定义联系人文件夹和如下所述的文件夹中的联系人。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-109">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="6f7c5-110">共享文件夹中获取联系人</span><span class="sxs-lookup"><span data-stu-id="6f7c5-110">Get a contact in the shared folder</span></span>

<span data-ttu-id="6f7c5-111">您可以与 John 共享 Garth 的自定义联系人文件夹中获取特定的联系人：</span><span class="sxs-lookup"><span data-stu-id="6f7c5-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="6f7c5-112">在操作成功完成，您将获取 HTTP 200 确定和[联系人](/graph/api/resources/contact?view=graph-rest-1.0)实例由标识`{id}`Garth 的共享联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-112">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="6f7c5-113">获取共享文件夹中的所有联系人</span><span class="sxs-lookup"><span data-stu-id="6f7c5-113">Get all contacts in the shared folder</span></span>

<span data-ttu-id="6f7c5-114">获取 Garth 的共享联系人文件夹中的所有联系人：</span><span class="sxs-lookup"><span data-stu-id="6f7c5-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="6f7c5-115">在操作成功完成，您将获取 HTTP 200 确定和共享联系人文件夹中 Garth 的[联系人](/graph/api/resources/contact?view=graph-rest-1.0)的实例的集合。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-115">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="6f7c5-116">获取共享文件夹</span><span class="sxs-lookup"><span data-stu-id="6f7c5-116">Get the shared folder</span></span>

<span data-ttu-id="6f7c5-117">获取与 John 共享 Garth 联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-117">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="6f7c5-118">在操作成功完成，您将获取 HTTP 200 确定，并表示 Garth 的[contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)实例共享联系人文件夹。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-118">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="6f7c5-119">如果 Garth 具有委派 John 其整个邮箱，应用相同的 GET 功能。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-119">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="6f7c5-120">如果 Garth 不具有与 John、 共享联系人文件夹，也没有有他代理其邮箱到 John，这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-120">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="6f7c5-121">后续步骤</span><span class="sxs-lookup"><span data-stu-id="6f7c5-121">Next steps</span></span>

<span data-ttu-id="6f7c5-122">详细了解以下信息：</span><span class="sxs-lookup"><span data-stu-id="6f7c5-122">Find out more about:</span></span>

- [<span data-ttu-id="6f7c5-123">为什么集成 Outlook 个人联系人</span><span class="sxs-lookup"><span data-stu-id="6f7c5-123">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="6f7c5-124">Microsoft Graph v1.0 中的[联系人 API](/graph/api/resources/contact?view=graph-rest-1.0) 。</span><span class="sxs-lookup"><span data-stu-id="6f7c5-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>