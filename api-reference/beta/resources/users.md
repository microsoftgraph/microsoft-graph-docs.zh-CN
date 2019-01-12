---
title: 在 Microsoft Graph 中与用户一起工作
description: 可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a5e1ed5a2403def740d92b9f77d57a58f6d1a3e6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912013"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="85377-103">在 Microsoft Graph 中与用户一起工作</span><span class="sxs-lookup"><span data-stu-id="85377-103">Working with users in Microsoft Graph</span></span>

> <span data-ttu-id="85377-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85377-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85377-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85377-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85377-106">可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。</span><span class="sxs-lookup"><span data-stu-id="85377-106">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="85377-107">通过 Microsoft Graph，你能以两种方式访问 用户</span><span class="sxs-lookup"><span data-stu-id="85377-107">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="85377-108">通过用户 ID，`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="85377-108">By their ID, `/users/{id}`</span></span> 
- <span data-ttu-id="85377-109">通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同</span><span class="sxs-lookup"><span data-stu-id="85377-109">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="85377-110">Authorization</span><span class="sxs-lookup"><span data-stu-id="85377-110">Authorization</span></span>
<span data-ttu-id="85377-p102">需要以下 [权限](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) 之一才能访问用户操作。用户可将前三个权限授予应用程序。其余权限只能由管理员授予应用。</span><span class="sxs-lookup"><span data-stu-id="85377-p102">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="85377-114">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="85377-114">User.ReadBasic.All</span></span>
- <span data-ttu-id="85377-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="85377-115">User.Read</span></span>
- <span data-ttu-id="85377-116">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85377-116">User.ReadWrite</span></span>
- <span data-ttu-id="85377-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="85377-117">User.Read.All</span></span>
- <span data-ttu-id="85377-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85377-118">User.ReadWrite.All</span></span>
- <span data-ttu-id="85377-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="85377-119">Directory.Read.All</span></span>
- <span data-ttu-id="85377-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85377-120">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="85377-121">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85377-121">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="85377-122">通用属性</span><span class="sxs-lookup"><span data-stu-id="85377-122">Common properties</span></span>

| <span data-ttu-id="85377-123">属性</span><span class="sxs-lookup"><span data-stu-id="85377-123">Property</span></span> | <span data-ttu-id="85377-124">说明</span><span class="sxs-lookup"><span data-stu-id="85377-124">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="85377-125">displayName</span><span class="sxs-lookup"><span data-stu-id="85377-125">displayName</span></span> | <span data-ttu-id="85377-126">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="85377-126">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="85377-127">givenName</span><span class="sxs-lookup"><span data-stu-id="85377-127">givenName</span></span>| <span data-ttu-id="85377-128">用户的名</span><span class="sxs-lookup"><span data-stu-id="85377-128">The first name of the user.</span></span> |
|<span data-ttu-id="85377-129">surname</span><span class="sxs-lookup"><span data-stu-id="85377-129">surname</span></span>| <span data-ttu-id="85377-130">用户的姓。</span><span class="sxs-lookup"><span data-stu-id="85377-130">The last name of the user.</span></span> |
|<span data-ttu-id="85377-131">mail</span><span class="sxs-lookup"><span data-stu-id="85377-131">mail</span></span>| <span data-ttu-id="85377-132">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="85377-132">The user's email address.</span></span> |
|<span data-ttu-id="85377-133">photo</span><span class="sxs-lookup"><span data-stu-id="85377-133">photo</span></span>| <span data-ttu-id="85377-134">用户配置文件照片。</span><span class="sxs-lookup"><span data-stu-id="85377-134">The user's profile photo.</span></span> |

<span data-ttu-id="85377-135">有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85377-135">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="85377-136">通用操作</span><span class="sxs-lookup"><span data-stu-id="85377-136">Common operations</span></span>
><span data-ttu-id="85377-137">**注意：** 某些操作需要其他权限。</span><span class="sxs-lookup"><span data-stu-id="85377-137">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="85377-138">路径</span><span class="sxs-lookup"><span data-stu-id="85377-138">Path</span></span>    | <span data-ttu-id="85377-139">说明</span><span class="sxs-lookup"><span data-stu-id="85377-139">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="85377-140">列出组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="85377-140">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="85377-141">通过 ID 获取特定用户。</span><span class="sxs-lookup"><span data-stu-id="85377-141">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="85377-142">获取用户个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="85377-142">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="85377-143">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="85377-143">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="85377-144">列出用户主收件箱中的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="85377-144">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="85377-145">列出用户日历中即将发生的事件。</span><span class="sxs-lookup"><span data-stu-id="85377-145">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="85377-146">获取用户 OneDrive 文件存储。</span><span class="sxs-lookup"><span data-stu-id="85377-146">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="85377-147">列出用户是其成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="85377-147">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="85377-148">列出了 Microsoft 小组成员的用户。</span><span class="sxs-lookup"><span data-stu-id="85377-148">Lists the Microsoft Teams that the user is a member of.</span></span> |
