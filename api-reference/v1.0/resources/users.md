---
title: 在 Microsoft Graph 中与用户一起工作
description: 可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: b0744662008b0b82167ce8779f478f260eedee57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033486"
---
# <a name="working-with-users-in-microsoft-graph"></a><span data-ttu-id="b740a-103">在 Microsoft Graph 中与用户一起工作</span><span class="sxs-lookup"><span data-stu-id="b740a-103">Working with users in Microsoft Graph</span></span>

<span data-ttu-id="b740a-104">可以使用 Microsoft Graph 构建基于用户、用户与其他用户和组的关系、用户邮件、日历和文件且有说服力的应用体验。</span><span class="sxs-lookup"><span data-stu-id="b740a-104">You can use Microsoft Graph to build compelling app experiences based on users, their relationships with other users and groups, and their mail, calendar, and files.</span></span>

<span data-ttu-id="b740a-105">通过 Microsoft Graph，你能以两种方式访问 [用户](user.md)</span><span class="sxs-lookup"><span data-stu-id="b740a-105">You can access [users](user.md) through Microsoft Graph in two ways:</span></span>

- <span data-ttu-id="b740a-106">通过用户 ID，`/users/{id | userPrincipalName}`</span><span class="sxs-lookup"><span data-stu-id="b740a-106">By their ID, `/users/{id | userPrincipalName}`</span></span> 
- <span data-ttu-id="b740a-107">通过使用已登录的用户的 `/me` 别名，这与 `/users/{signed-in user's id}` 相同</span><span class="sxs-lookup"><span data-stu-id="b740a-107">By using the `/me` alias for the signed-in user, which is the same as `/users/{signed-in user's id}`</span></span>

## <a name="authorization"></a><span data-ttu-id="b740a-108">授权</span><span class="sxs-lookup"><span data-stu-id="b740a-108">Authorization</span></span>

<span data-ttu-id="b740a-p101">需要以下 [权限](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) 之一才能访问用户操作。用户可将前三个权限授予应用程序。其余权限只能由管理员授予应用。</span><span class="sxs-lookup"><span data-stu-id="b740a-p101">One of the following [permissions](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to access user operations. The first three permissions can be granted to an app by a user. The rest can only be granted to an app by the administrator.</span></span>

- <span data-ttu-id="b740a-112">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="b740a-112">User.ReadBasic.All</span></span>
- <span data-ttu-id="b740a-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="b740a-113">User.Read</span></span>
- <span data-ttu-id="b740a-114">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b740a-114">User.ReadWrite</span></span>
- <span data-ttu-id="b740a-115">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="b740a-115">User.Read.All</span></span>
- <span data-ttu-id="b740a-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b740a-116">User.ReadWrite.All</span></span>
- <span data-ttu-id="b740a-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b740a-117">Directory.Read.All</span></span>
- <span data-ttu-id="b740a-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b740a-118">Directory.ReadWrite.All</span></span>
- <span data-ttu-id="b740a-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b740a-119">Directory.AccessAsUser.All</span></span>

## <a name="common-properties"></a><span data-ttu-id="b740a-120">通用属性</span><span class="sxs-lookup"><span data-stu-id="b740a-120">Common properties</span></span>

<span data-ttu-id="b740a-121">以下内容表示获取或列出用户时返回的属性的默认集。</span><span class="sxs-lookup"><span data-stu-id="b740a-121">The following represent the default set of properties that are returned when getting a user or listing users.</span></span> <span data-ttu-id="b740a-122">这些是所有可用属性的子集。</span><span class="sxs-lookup"><span data-stu-id="b740a-122">These are a subset of all available properties.</span></span> <span data-ttu-id="b740a-123">要获取更多用户属性，请使用 `$select` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="b740a-123">To get more user properties, use the `$select` query parameter.</span></span> 

|<span data-ttu-id="b740a-124">属性</span><span class="sxs-lookup"><span data-stu-id="b740a-124">Property</span></span> |<span data-ttu-id="b740a-125">说明</span><span class="sxs-lookup"><span data-stu-id="b740a-125">Description</span></span> |
|:----------|:-------------|
|<span data-ttu-id="b740a-126">id</span><span class="sxs-lookup"><span data-stu-id="b740a-126">id</span></span> | <span data-ttu-id="b740a-127">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b740a-127">The unique identifier for the user.</span></span>|
|<span data-ttu-id="b740a-128">businessPhones</span><span class="sxs-lookup"><span data-stu-id="b740a-128">businessPhones</span></span> | <span data-ttu-id="b740a-129">用户的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b740a-129">The user's phone numbers.</span></span>|
|<span data-ttu-id="b740a-130">displayName</span><span class="sxs-lookup"><span data-stu-id="b740a-130">displayName</span></span> | <span data-ttu-id="b740a-131">用户通讯簿中显示的名称。</span><span class="sxs-lookup"><span data-stu-id="b740a-131">The name displayed in the address book for the user.</span></span>|
|<span data-ttu-id="b740a-132">givenName</span><span class="sxs-lookup"><span data-stu-id="b740a-132">givenName</span></span>| <span data-ttu-id="b740a-133">用户的名</span><span class="sxs-lookup"><span data-stu-id="b740a-133">The first name of the user.</span></span> |
|<span data-ttu-id="b740a-134">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b740a-134">jobTitle</span></span> | <span data-ttu-id="b740a-135">用户的职务。</span><span class="sxs-lookup"><span data-stu-id="b740a-135">The user's job title.</span></span>|
|<span data-ttu-id="b740a-136">mail</span><span class="sxs-lookup"><span data-stu-id="b740a-136">mail</span></span>| <span data-ttu-id="b740a-137">用户的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b740a-137">The user's email address.</span></span> |
|<span data-ttu-id="b740a-138">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b740a-138">mobilePhone</span></span> | <span data-ttu-id="b740a-139">用户的手机号码。</span><span class="sxs-lookup"><span data-stu-id="b740a-139">The user's cellphone number.</span></span>|
|<span data-ttu-id="b740a-140">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b740a-140">officeLocation</span></span> | <span data-ttu-id="b740a-141">用户的办公地址。</span><span class="sxs-lookup"><span data-stu-id="b740a-141">The user's physical office location.</span></span>|
|<span data-ttu-id="b740a-142">preferredLanguage</span><span class="sxs-lookup"><span data-stu-id="b740a-142">preferredLanguage</span></span> | <span data-ttu-id="b740a-143">用户的语言首选项。</span><span class="sxs-lookup"><span data-stu-id="b740a-143">The user's language of preference.</span></span>|
|<span data-ttu-id="b740a-144">surname</span><span class="sxs-lookup"><span data-stu-id="b740a-144">surname</span></span>| <span data-ttu-id="b740a-145">用户的姓。</span><span class="sxs-lookup"><span data-stu-id="b740a-145">The last name of the user.</span></span> |
|<span data-ttu-id="b740a-146">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b740a-146">userPrincipalName</span></span>| <span data-ttu-id="b740a-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b740a-147">The user's principal name.</span></span> |

<br/>

<span data-ttu-id="b740a-148">有关详细信息及所有属性的列表，请参阅 [user](user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b740a-148">For details and a list of all the properties, see the [user](user.md) object.</span></span>

## <a name="common-operations"></a><span data-ttu-id="b740a-149">通用操作</span><span class="sxs-lookup"><span data-stu-id="b740a-149">Common operations</span></span>

> <span data-ttu-id="b740a-150">**注意：** 某些操作需要其他权限。</span><span class="sxs-lookup"><span data-stu-id="b740a-150">**Note:** Some of these operations require additional permissions.</span></span>

| <span data-ttu-id="b740a-151">路径</span><span class="sxs-lookup"><span data-stu-id="b740a-151">Path</span></span>    | <span data-ttu-id="b740a-152">说明</span><span class="sxs-lookup"><span data-stu-id="b740a-152">Description</span></span> |
|:---------|:-------------|
|[`/users`](../api/user-list.md) | <span data-ttu-id="b740a-153">列出组织中的用户。</span><span class="sxs-lookup"><span data-stu-id="b740a-153">Lists users in the organization.</span></span> |
|[`/users/{id}`](../api/user-get.md) | <span data-ttu-id="b740a-154">通过 ID 获取特定用户。</span><span class="sxs-lookup"><span data-stu-id="b740a-154">Gets a specific user by id.</span></span> |
|[`/users/{id}/photo/$value`](../api/profilephoto-get.md)| <span data-ttu-id="b740a-155">获取用户个人资料照片。</span><span class="sxs-lookup"><span data-stu-id="b740a-155">Gets the user's profile photo.</span></span> |
|[`/users/{id}/manager`](../api/user-list-manager.md) | <span data-ttu-id="b740a-156">获取用户的经理。</span><span class="sxs-lookup"><span data-stu-id="b740a-156">Gets the user's manager.</span></span> |
|[`/users/{id}/messages`](../api/user-list-messages.md)| <span data-ttu-id="b740a-157">列出用户主收件箱中的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="b740a-157">Lists the user's email messages in their primary inbox.</span></span> |
|[`/users/{id}/events`](../api/user-list-events.md) | <span data-ttu-id="b740a-158">列出用户日历中即将发生的事件。</span><span class="sxs-lookup"><span data-stu-id="b740a-158">Lists the user's upcoming events in their calendar.</span></span> |
|[`/users/{id}/drive`](../api/drive-get.md)| <span data-ttu-id="b740a-159">获取用户 OneDrive 文件存储。</span><span class="sxs-lookup"><span data-stu-id="b740a-159">Gets the user's OneDrive file store.</span></span> |
|[`/users/{id}/memberOf`](../api/user-list-memberof.md)| <span data-ttu-id="b740a-160">列出用户是其成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="b740a-160">Lists the groups that the user is a member of.</span></span> |
