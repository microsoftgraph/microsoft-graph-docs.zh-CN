---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00afa9e91d350fedd023646ab952db641addb9f7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730349"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="90d34-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="90d34-103">educationRoot resource type</span></span>

<span data-ttu-id="90d34-104">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="90d34-104">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="90d34-105">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="90d34-105">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="90d34-106">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="90d34-106">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="90d34-107">方法</span><span class="sxs-lookup"><span data-stu-id="90d34-107">Methods</span></span>

| <span data-ttu-id="90d34-108">方法</span><span class="sxs-lookup"><span data-stu-id="90d34-108">Method</span></span>           | <span data-ttu-id="90d34-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="90d34-109">Return Type</span></span>    |<span data-ttu-id="90d34-110">说明</span><span class="sxs-lookup"><span data-stu-id="90d34-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90d34-111">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="90d34-111">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="90d34-112">educationClass</span><span class="sxs-lookup"><span data-stu-id="90d34-112">educationClass</span></span>](educationclass.md)| <span data-ttu-id="90d34-113">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="90d34-113">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="90d34-114">List classes</span><span class="sxs-lookup"><span data-stu-id="90d34-114">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="90d34-115">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90d34-115">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="90d34-116">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90d34-116">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="90d34-117">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="90d34-117">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="90d34-118">educationSchool</span><span class="sxs-lookup"><span data-stu-id="90d34-118">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="90d34-119">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="90d34-119">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="90d34-120">List schools</span><span class="sxs-lookup"><span data-stu-id="90d34-120">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="90d34-121">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90d34-121">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="90d34-122">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90d34-122">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="90d34-123">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="90d34-123">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="90d34-124">educationUser</span><span class="sxs-lookup"><span data-stu-id="90d34-124">educationUser</span></span>](educationuser.md)| <span data-ttu-id="90d34-125">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="90d34-125">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="90d34-126">List users</span><span class="sxs-lookup"><span data-stu-id="90d34-126">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="90d34-127">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90d34-127">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="90d34-128">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90d34-128">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="90d34-129">属性</span><span class="sxs-lookup"><span data-stu-id="90d34-129">Properties</span></span>
<span data-ttu-id="90d34-130">无。</span><span class="sxs-lookup"><span data-stu-id="90d34-130">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="90d34-131">关系</span><span class="sxs-lookup"><span data-stu-id="90d34-131">Relationships</span></span>
| <span data-ttu-id="90d34-132">关系</span><span class="sxs-lookup"><span data-stu-id="90d34-132">Relationship</span></span> | <span data-ttu-id="90d34-133">类型</span><span class="sxs-lookup"><span data-stu-id="90d34-133">Type</span></span>   |<span data-ttu-id="90d34-134">说明</span><span class="sxs-lookup"><span data-stu-id="90d34-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90d34-135">classes</span><span class="sxs-lookup"><span data-stu-id="90d34-135">classes</span></span>|<span data-ttu-id="90d34-136">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90d34-136">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="90d34-137">只读。</span><span class="sxs-lookup"><span data-stu-id="90d34-137">Read-only.</span></span> <span data-ttu-id="90d34-138">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90d34-138">Nullable.</span></span>|
|<span data-ttu-id="90d34-139">me</span><span class="sxs-lookup"><span data-stu-id="90d34-139">me</span></span>|[<span data-ttu-id="90d34-140">educationUser</span><span class="sxs-lookup"><span data-stu-id="90d34-140">educationUser</span></span>](educationuser.md)| <span data-ttu-id="90d34-141">只读。</span><span class="sxs-lookup"><span data-stu-id="90d34-141">Read-only.</span></span> <span data-ttu-id="90d34-142">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="90d34-142">Nullable.</span></span>|
|<span data-ttu-id="90d34-143">schools</span><span class="sxs-lookup"><span data-stu-id="90d34-143">schools</span></span>|<span data-ttu-id="90d34-144">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90d34-144">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="90d34-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="90d34-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="90d34-147">users</span><span class="sxs-lookup"><span data-stu-id="90d34-147">users</span></span>|<span data-ttu-id="90d34-148">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="90d34-148">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="90d34-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="90d34-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90d34-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90d34-151">JSON representation</span></span>
<span data-ttu-id="90d34-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90d34-152">Here is a JSON representation of the resource.</span></span>

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


# <a name="httptabhttp"></a>[<span data-ttu-id="90d34-153">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="90d34-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="90d34-154">C#</span><span class="sxs-lookup"><span data-stu-id="90d34-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90d34-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90d34-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="90d34-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="90d34-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="90d34-157">Java</span><span class="sxs-lookup"><span data-stu-id="90d34-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-education-java-snippets.md)]
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
