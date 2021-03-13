---
title: 在 Microsoft Graph 中与用户一起工作
description: 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
localization_priority: Priority
author: jpettere
ms.prod: users
doc_type: conceptualPageType
ms.openlocfilehash: 7c1d2df4e6d1795e1cc4965e8bfcfe4bf4e4d9c8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761782"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="225dd-103">在 Microsoft Graph 中与用户一起工作</span><span class="sxs-lookup"><span data-stu-id="225dd-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="225dd-104">可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。</span><span class="sxs-lookup"><span data-stu-id="225dd-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="225dd-105">通过 Microsoft Graph，你能以两种方式访问用户：</span><span class="sxs-lookup"><span data-stu-id="225dd-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="225dd-106">通过用户 ID，`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="225dd-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="225dd-107">通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同</span><span class="sxs-lookup"><span data-stu-id="225dd-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="225dd-108">授权</span><span class="sxs-lookup"><span data-stu-id="225dd-108">Authorization</span></span>

<span data-ttu-id="225dd-p101">需要以下 [权限](/graph/permissions-reference) 之一才能访问用户操作。用户可将前三个权限授予应用程序。其余权限只能由管理员授予应用。</span><span class="sxs-lookup"><span data-stu-id="225dd-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="225dd-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="225dd-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="225dd-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="225dd-113">User.Read</span></span>
- <span data-ttu-id="225dd-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="225dd-114">User.ReadWrite</span></span>
- <span data-ttu-id="225dd-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="225dd-115">User.Read.All</span></span>
- <span data-ttu-id="225dd-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225dd-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="225dd-117">User.ManageIdentities.All</span><span class="sxs-lookup"><span data-stu-id="225dd-117">User.ManageIdentities.All</span></span>
- <span data-ttu-id="225dd-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="225dd-118">Directory.Read.All</span></span>
- <span data-ttu-id="225dd-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="225dd-119">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="225dd-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="225dd-120">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="225dd-121">通用属性</span><span class="sxs-lookup"><span data-stu-id="225dd-121">Common properties</span></span>

| <span data-ttu-id="225dd-122">属性</span><span class="sxs-lookup"><span data-stu-id="225dd-122">Property</span></span> | <span data-ttu-id="225dd-123">说明</span><span class="sxs-lookup"><span data-stu-id="225dd-123">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="225dd-124">displayName</span><span class="sxs-lookup"><span data-stu-id="225dd-124">displayName</span></span> | <span data-ttu-id="225dd-125">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="225dd-125">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="225dd-126">givenName</span><span class="sxs-lookup"><span data-stu-id="225dd-126">givenName</span></span>| <span data-ttu-id="225dd-127">用户的名。</span><span class="sxs-lookup"><span data-stu-id="225dd-127">The first name of the user.</span></span> |
|<span data-ttu-id="225dd-128">surname</span><span class="sxs-lookup"><span data-stu-id="225dd-128">surname</span></span>| <span data-ttu-id="225dd-129">用户的姓。</span><span class="sxs-lookup"><span data-stu-id="225dd-129">The last name of the user.</span></span> |
|<span data-ttu-id="225dd-130">mail</span><span class="sxs-lookup"><span data-stu-id="225dd-130">mail</span></span>| <span data-ttu-id="225dd-131">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="225dd-131">The user's email address.</span></span> |
|<span data-ttu-id="225dd-132">photo</span><span class="sxs-lookup"><span data-stu-id="225dd-132">photo</span></span>| <span data-ttu-id="225dd-133">用户的个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="225dd-133">The user's profile photo.</span></span> |

<span data-ttu-id="225dd-134">有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="225dd-134">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="225dd-135">通用操作</span><span class="sxs-lookup"><span data-stu-id="225dd-135">Common operations</span></span>

><span data-ttu-id="225dd-136">**注意：** 某些操作需要其他权限。</span><span class="sxs-lookup"><span data-stu-id="225dd-136">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="225dd-137">路径</span><span class="sxs-lookup"><span data-stu-id="225dd-137">Path</span></span>    | <span data-ttu-id="225dd-138">说明</span><span class="sxs-lookup"><span data-stu-id="225dd-138">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="225dd-139">列出组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="225dd-139">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="225dd-140">通过 ID 获取特定用户。</span><span class="sxs-lookup"><span data-stu-id="225dd-140">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="225dd-141">获取用户个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="225dd-141">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="225dd-142">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="225dd-142">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="225dd-143">列出用户主收件箱中的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="225dd-143">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="225dd-144">列出用户日历中即将发生的事件。</span><span class="sxs-lookup"><span data-stu-id="225dd-144">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="225dd-145">获取用户 OneDrive 文件存储。</span><span class="sxs-lookup"><span data-stu-id="225dd-145">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="225dd-146">列出用户是其成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="225dd-146">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="225dd-147">列出用户所属的 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="225dd-147">Lists the Microsoft Teams that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="225dd-148">最近更新</span><span class="sxs-lookup"><span data-stu-id="225dd-148">What's new</span></span>
<span data-ttu-id="225dd-149">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="225dd-149">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>