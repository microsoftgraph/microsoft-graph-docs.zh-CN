---
title: 在 Microsoft Graph 中与用户一起工作
description: 可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f1a08e008f1de343ca6cf4986006c43c7e115af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518427"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="be626-103">在 Microsoft Graph 中与用户一起工作</span><span class="sxs-lookup"><span data-stu-id="be626-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be626-104">可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。</span><span class="sxs-lookup"><span data-stu-id="be626-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="be626-105">通过 Microsoft Graph，你能以两种方式访问用户：</span><span class="sxs-lookup"><span data-stu-id="be626-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="be626-106">通过用户 ID，`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="be626-106">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="be626-107">通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同</span><span class="sxs-lookup"><span data-stu-id="be626-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="be626-108">授权</span><span class="sxs-lookup"><span data-stu-id="be626-108">Authorization</span></span>
<span data-ttu-id="be626-p101">需要以下 [权限](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) 之一才能访问用户操作。用户可将前三个权限授予应用程序。其余权限只能由管理员授予应用。</span><span class="sxs-lookup"><span data-stu-id="be626-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="be626-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="be626-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="be626-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="be626-113">User.Read</span></span>
- <span data-ttu-id="be626-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="be626-114">User.ReadWrite</span></span>
- <span data-ttu-id="be626-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="be626-115">User.Read.All</span></span>
- <span data-ttu-id="be626-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be626-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="be626-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="be626-117">Directory.Read.All</span></span>
- <span data-ttu-id="be626-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be626-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="be626-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="be626-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="be626-120">通用属性</span><span class="sxs-lookup"><span data-stu-id="be626-120">Common properties</span></span>

| <span data-ttu-id="be626-121">属性</span><span class="sxs-lookup"><span data-stu-id="be626-121">Property</span></span> | <span data-ttu-id="be626-122">说明</span><span class="sxs-lookup"><span data-stu-id="be626-122">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="be626-123">displayName</span><span class="sxs-lookup"><span data-stu-id="be626-123">displayName</span></span> | <span data-ttu-id="be626-124">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="be626-124">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="be626-125">givenName</span><span class="sxs-lookup"><span data-stu-id="be626-125">givenName</span></span>| <span data-ttu-id="be626-126">用户的名。</span><span class="sxs-lookup"><span data-stu-id="be626-126">The first name of the user.</span></span> |
|<span data-ttu-id="be626-127">surname</span><span class="sxs-lookup"><span data-stu-id="be626-127">surname</span></span>| <span data-ttu-id="be626-128">用户的姓。</span><span class="sxs-lookup"><span data-stu-id="be626-128">The last name of the user.</span></span> |
|<span data-ttu-id="be626-129">mail</span><span class="sxs-lookup"><span data-stu-id="be626-129">mail</span></span>| <span data-ttu-id="be626-130">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="be626-130">The user's email address.</span></span> |
|<span data-ttu-id="be626-131">photo</span><span class="sxs-lookup"><span data-stu-id="be626-131">photo</span></span>| <span data-ttu-id="be626-132">用户的个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="be626-132">The user's profile photo.</span></span> |

<span data-ttu-id="be626-133">有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="be626-133">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="be626-134">通用操作</span><span class="sxs-lookup"><span data-stu-id="be626-134">Common operations</span></span>
><span data-ttu-id="be626-135">**注意：** 某些操作需要其他权限。</span><span class="sxs-lookup"><span data-stu-id="be626-135">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="be626-136">路径</span><span class="sxs-lookup"><span data-stu-id="be626-136">Path</span></span>    | <span data-ttu-id="be626-137">说明</span><span class="sxs-lookup"><span data-stu-id="be626-137">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="be626-138">列出组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="be626-138">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="be626-139">通过 ID 获取特定用户。</span><span class="sxs-lookup"><span data-stu-id="be626-139">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="be626-140">获取用户个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="be626-140">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="be626-141">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="be626-141">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="be626-142">列出用户主收件箱中的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="be626-142">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="be626-143">列出用户日历中即将发生的事件。</span><span class="sxs-lookup"><span data-stu-id="be626-143">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="be626-144">获取用户 OneDrive 文件存储。</span><span class="sxs-lookup"><span data-stu-id="be626-144">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="be626-145">列出用户是其成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="be626-145">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="be626-146">列出用户所属的 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="be626-146">Lists the Microsoft Teams that the user is a member of.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
