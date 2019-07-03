---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84b7312515174c19837a5cda3fa3ffb466f65c23
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458752"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="21726-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="21726-103">educationRoot resource type</span></span>

<span data-ttu-id="21726-104">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="21726-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="21726-105">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="21726-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="21726-106">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="21726-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="21726-107">方法</span><span class="sxs-lookup"><span data-stu-id="21726-107">Methods</span></span>

| <span data-ttu-id="21726-108">方法</span><span class="sxs-lookup"><span data-stu-id="21726-108">Method</span></span>           | <span data-ttu-id="21726-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="21726-109">Return Type</span></span>    |<span data-ttu-id="21726-110">说明</span><span class="sxs-lookup"><span data-stu-id="21726-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21726-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="21726-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="21726-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="21726-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="21726-113">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="21726-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="21726-114">List classes</span><span class="sxs-lookup"><span data-stu-id="21726-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="21726-115">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21726-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="21726-116">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="21726-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="21726-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="21726-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="21726-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="21726-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="21726-119">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="21726-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="21726-120">List schools</span><span class="sxs-lookup"><span data-stu-id="21726-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="21726-121">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21726-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="21726-122">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="21726-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="21726-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="21726-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="21726-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="21726-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="21726-125">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="21726-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="21726-126">List users</span><span class="sxs-lookup"><span data-stu-id="21726-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="21726-127">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21726-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="21726-128">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="21726-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="21726-129">属性</span><span class="sxs-lookup"><span data-stu-id="21726-129">Properties</span></span>
<span data-ttu-id="21726-130">无。</span><span class="sxs-lookup"><span data-stu-id="21726-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="21726-131">关系</span><span class="sxs-lookup"><span data-stu-id="21726-131">Relationships</span></span>
| <span data-ttu-id="21726-132">关系</span><span class="sxs-lookup"><span data-stu-id="21726-132">Relationship</span></span> | <span data-ttu-id="21726-133">类型</span><span class="sxs-lookup"><span data-stu-id="21726-133">Type</span></span>   |<span data-ttu-id="21726-134">说明</span><span class="sxs-lookup"><span data-stu-id="21726-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21726-135">classes</span><span class="sxs-lookup"><span data-stu-id="21726-135">classes</span></span>|<span data-ttu-id="21726-136">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21726-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="21726-137">只读。</span><span class="sxs-lookup"><span data-stu-id="21726-137">Read-only.</span></span> <span data-ttu-id="21726-138">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="21726-138">Nullable.</span></span>|
|<span data-ttu-id="21726-139">me</span><span class="sxs-lookup"><span data-stu-id="21726-139">me</span></span>|[<span data-ttu-id="21726-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="21726-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="21726-141">只读。</span><span class="sxs-lookup"><span data-stu-id="21726-141">Read-only.</span></span> <span data-ttu-id="21726-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="21726-142">Nullable.</span></span>|
|<span data-ttu-id="21726-143">schools</span><span class="sxs-lookup"><span data-stu-id="21726-143">schools</span></span>|<span data-ttu-id="21726-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21726-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="21726-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="21726-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="21726-147">users</span><span class="sxs-lookup"><span data-stu-id="21726-147">users</span></span>|<span data-ttu-id="21726-148">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="21726-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="21726-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="21726-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21726-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21726-151">JSON representation</span></span>
<span data-ttu-id="21726-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21726-152">Here is a JSON representation of the resource.</span></span>

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


# <a name="httptabhttp"></a>[<span data-ttu-id="21726-153">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="21726-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21726-154">C#</span><span class="sxs-lookup"><span data-stu-id="21726-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21726-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="21726-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21726-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="21726-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
  "tocPath": "",
  "suppressions": [
  ]
}-->
