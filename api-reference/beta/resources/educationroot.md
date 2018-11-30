---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
ms.openlocfilehash: 01845df878d5e6a4fe01cb29f73d73b6980cfa9a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042507"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="90405-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="90405-103">educationRoot resource type</span></span>

> <span data-ttu-id="90405-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="90405-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90405-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="90405-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90405-106">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="90405-106">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="90405-107">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="90405-107">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="90405-108">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="90405-108">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="90405-109">方法</span><span class="sxs-lookup"><span data-stu-id="90405-109">Methods</span></span>

| <span data-ttu-id="90405-110">方法</span><span class="sxs-lookup"><span data-stu-id="90405-110">Method</span></span>           | <span data-ttu-id="90405-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="90405-111">Return Type</span></span>    |<span data-ttu-id="90405-112">说明</span><span class="sxs-lookup"><span data-stu-id="90405-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90405-113">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="90405-113">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="90405-114">educationClass</span><span class="sxs-lookup"><span data-stu-id="90405-114">educationClass</span></span>](educationclass.md)| <span data-ttu-id="90405-115">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="90405-115">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="90405-116">List classes</span><span class="sxs-lookup"><span data-stu-id="90405-116">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="90405-117">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90405-117">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="90405-118">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90405-118">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="90405-119">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="90405-119">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="90405-120">educationSchool</span><span class="sxs-lookup"><span data-stu-id="90405-120">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="90405-121">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="90405-121">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="90405-122">List schools</span><span class="sxs-lookup"><span data-stu-id="90405-122">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="90405-123">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90405-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="90405-124">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90405-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="90405-125">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="90405-125">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="90405-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="90405-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="90405-127">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="90405-127">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="90405-128">List users</span><span class="sxs-lookup"><span data-stu-id="90405-128">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="90405-129">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90405-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="90405-130">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90405-130">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="90405-131">属性</span><span class="sxs-lookup"><span data-stu-id="90405-131">Properties</span></span>
<span data-ttu-id="90405-132">无。</span><span class="sxs-lookup"><span data-stu-id="90405-132">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="90405-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="90405-133">Relationships</span></span>
| <span data-ttu-id="90405-134">关系</span><span class="sxs-lookup"><span data-stu-id="90405-134">Relationship</span></span> | <span data-ttu-id="90405-135">类型</span><span class="sxs-lookup"><span data-stu-id="90405-135">Type</span></span>   |<span data-ttu-id="90405-136">说明</span><span class="sxs-lookup"><span data-stu-id="90405-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90405-137">classes</span><span class="sxs-lookup"><span data-stu-id="90405-137">classes</span></span>|<span data-ttu-id="90405-138">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90405-138">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="90405-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="90405-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90405-141">me</span><span class="sxs-lookup"><span data-stu-id="90405-141">me</span></span>|[<span data-ttu-id="90405-142">educationUser</span><span class="sxs-lookup"><span data-stu-id="90405-142">educationUser</span></span>](educationuser.md)| <span data-ttu-id="90405-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="90405-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90405-145">schools</span><span class="sxs-lookup"><span data-stu-id="90405-145">schools</span></span>|<span data-ttu-id="90405-146">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90405-146">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="90405-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="90405-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90405-149">users</span><span class="sxs-lookup"><span data-stu-id="90405-149">users</span></span>|<span data-ttu-id="90405-150">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90405-150">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="90405-p106">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="90405-p106">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->