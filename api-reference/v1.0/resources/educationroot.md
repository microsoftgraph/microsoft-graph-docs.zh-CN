---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5b9f17cf82c6839a95f1fd81405aa675e0f4d6ba
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943198"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="e295e-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="e295e-103">educationRoot resource type</span></span>

<span data-ttu-id="e295e-104">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="e295e-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="e295e-105">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="e295e-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="e295e-106">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="e295e-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="e295e-107">方法</span><span class="sxs-lookup"><span data-stu-id="e295e-107">Methods</span></span>

| <span data-ttu-id="e295e-108">方法</span><span class="sxs-lookup"><span data-stu-id="e295e-108">Method</span></span>           | <span data-ttu-id="e295e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e295e-109">Return Type</span></span>    |<span data-ttu-id="e295e-110">说明</span><span class="sxs-lookup"><span data-stu-id="e295e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e295e-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="e295e-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="e295e-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="e295e-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="e295e-113">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="e295e-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="e295e-114">List classes</span><span class="sxs-lookup"><span data-stu-id="e295e-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="e295e-115">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e295e-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e295e-116">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e295e-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="e295e-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="e295e-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="e295e-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="e295e-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="e295e-119">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="e295e-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="e295e-120">List schools</span><span class="sxs-lookup"><span data-stu-id="e295e-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="e295e-121">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e295e-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e295e-122">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e295e-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="e295e-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="e295e-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="e295e-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="e295e-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e295e-125">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="e295e-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="e295e-126">List users</span><span class="sxs-lookup"><span data-stu-id="e295e-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="e295e-127">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e295e-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e295e-128">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e295e-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e295e-129">属性</span><span class="sxs-lookup"><span data-stu-id="e295e-129">Properties</span></span>
<span data-ttu-id="e295e-130">无。</span><span class="sxs-lookup"><span data-stu-id="e295e-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e295e-131">Relationships</span><span class="sxs-lookup"><span data-stu-id="e295e-131">Relationships</span></span>
| <span data-ttu-id="e295e-132">关系</span><span class="sxs-lookup"><span data-stu-id="e295e-132">Relationship</span></span> | <span data-ttu-id="e295e-133">类型</span><span class="sxs-lookup"><span data-stu-id="e295e-133">Type</span></span>   |<span data-ttu-id="e295e-134">说明</span><span class="sxs-lookup"><span data-stu-id="e295e-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e295e-135">classes</span><span class="sxs-lookup"><span data-stu-id="e295e-135">classes</span></span>|<span data-ttu-id="e295e-136">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e295e-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="e295e-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e295e-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e295e-139">me</span><span class="sxs-lookup"><span data-stu-id="e295e-139">me</span></span>|[<span data-ttu-id="e295e-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="e295e-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="e295e-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e295e-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e295e-143">schools</span><span class="sxs-lookup"><span data-stu-id="e295e-143">schools</span></span>|<span data-ttu-id="e295e-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e295e-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="e295e-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e295e-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="e295e-147">users</span><span class="sxs-lookup"><span data-stu-id="e295e-147">users</span></span>|<span data-ttu-id="e295e-148">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e295e-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="e295e-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e295e-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e295e-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e295e-151">JSON representation</span></span>
<span data-ttu-id="e295e-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e295e-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
