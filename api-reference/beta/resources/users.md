---
title: 在 Microsoft Graph 中与用户一起工作
description: 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
localization_priority: Priority
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: c18731042d9d86479c5658f0a0f38a38d23bdb0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719820"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="4fb90-103">在 Microsoft Graph 中与用户一起工作</span><span class="sxs-lookup"><span data-stu-id="4fb90-103">Working with users in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4fb90-104">可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。</span><span class="sxs-lookup"><span data-stu-id="4fb90-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="4fb90-105">通过 Microsoft Graph，你能以两种方式访问用户：</span><span class="sxs-lookup"><span data-stu-id="4fb90-105">You can access users through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="4fb90-106">通过用户 ID，`/users/{id}`</span><span class="sxs-lookup"><span data-stu-id="4fb90-106">By their ID, `/users/{id}`</span></span>
- <span data-ttu-id="4fb90-107">通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同</span><span class="sxs-lookup"><span data-stu-id="4fb90-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="4fb90-108">授权</span><span class="sxs-lookup"><span data-stu-id="4fb90-108">Authorization</span></span>

<span data-ttu-id="4fb90-p101">需要以下 [权限](/graph/permissions-reference) 之一才能访问用户操作。用户可将前三个权限授予应用程序。其余权限只能由管理员授予应用。</span><span class="sxs-lookup"><span data-stu-id="4fb90-p101">One of the following [permissions](/graph/permissions-reference) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="4fb90-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="4fb90-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="4fb90-113">User.Read</span></span>
- <span data-ttu-id="4fb90-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4fb90-114">User.ReadWrite</span></span>
- <span data-ttu-id="4fb90-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-115">User.Read.All</span></span>
- <span data-ttu-id="4fb90-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="4fb90-117">User.ManageIdentities.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-117">User.ManageIdentities.All</span></span>
- <span data-ttu-id="4fb90-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-118">Directory.Read.All</span></span>
- <span data-ttu-id="4fb90-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-119">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="4fb90-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4fb90-120">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="4fb90-121">通用属性</span><span class="sxs-lookup"><span data-stu-id="4fb90-121">Common properties</span></span>

| <span data-ttu-id="4fb90-122">属性</span><span class="sxs-lookup"><span data-stu-id="4fb90-122">Property</span></span> | <span data-ttu-id="4fb90-123">说明</span><span class="sxs-lookup"><span data-stu-id="4fb90-123">Description</span></span> |
|----------|-------------|
| <span data-ttu-id="4fb90-124">displayName</span><span class="sxs-lookup"><span data-stu-id="4fb90-124">displayName</span></span> | <span data-ttu-id="4fb90-125">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="4fb90-125">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="4fb90-126">givenName</span><span class="sxs-lookup"><span data-stu-id="4fb90-126">givenName</span></span>| <span data-ttu-id="4fb90-127">用户的名。</span><span class="sxs-lookup"><span data-stu-id="4fb90-127">The first name of the user.</span></span> |
|<span data-ttu-id="4fb90-128">surname</span><span class="sxs-lookup"><span data-stu-id="4fb90-128">surname</span></span>| <span data-ttu-id="4fb90-129">用户的姓。</span><span class="sxs-lookup"><span data-stu-id="4fb90-129">The last name of the user.</span></span> |
|<span data-ttu-id="4fb90-130">mail</span><span class="sxs-lookup"><span data-stu-id="4fb90-130">mail</span></span>| <span data-ttu-id="4fb90-131">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4fb90-131">The user's email address.</span></span> |
|<span data-ttu-id="4fb90-132">photo</span><span class="sxs-lookup"><span data-stu-id="4fb90-132">photo</span></span>| <span data-ttu-id="4fb90-133">用户的个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="4fb90-133">The user's profile photo.</span></span> |

<span data-ttu-id="4fb90-134">有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fb90-134">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="4fb90-135">通用操作</span><span class="sxs-lookup"><span data-stu-id="4fb90-135">Common operations</span></span>

><span data-ttu-id="4fb90-136">**注意：** 某些操作需要其他权限。</span><span class="sxs-lookup"><span data-stu-id="4fb90-136">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="4fb90-137">路径</span><span class="sxs-lookup"><span data-stu-id="4fb90-137">Path</span></span>    | <span data-ttu-id="4fb90-138">说明</span><span class="sxs-lookup"><span data-stu-id="4fb90-138">Description</span></span> |
|---------|-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="4fb90-139">列出组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="4fb90-139">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="4fb90-140">通过 ID 获取特定用户。</span><span class="sxs-lookup"><span data-stu-id="4fb90-140">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="4fb90-141">获取用户个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="4fb90-141">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="4fb90-142">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="4fb90-142">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="4fb90-143">列出用户主收件箱中的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="4fb90-143">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="4fb90-144">列出用户日历中即将发生的事件。</span><span class="sxs-lookup"><span data-stu-id="4fb90-144">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="4fb90-145">获取用户 OneDrive 文件存储。</span><span class="sxs-lookup"><span data-stu-id="4fb90-145">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="4fb90-146">列出用户是其成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="4fb90-146">Lists the groups that the user is a member of.</span></span> |
|[`/users/{id}/joinedTeams`](../api/user-list-joinedteams.md)| <span data-ttu-id="4fb90-147">列出用户所属的 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="4fb90-147">Lists the Microsoft Teams that the user is a member of.</span></span> |

## <a name="whats-new"></a><span data-ttu-id="4fb90-148">最近更新</span><span class="sxs-lookup"><span data-stu-id="4fb90-148">What's new</span></span>
<span data-ttu-id="4fb90-149">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="4fb90-149">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>