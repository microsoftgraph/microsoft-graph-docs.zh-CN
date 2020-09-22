---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5f93b35dc48087b8d40db0cc3eabc2ba3ba10c8b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032682"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="704b8-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="704b8-103">educationRoot resource type</span></span>

<span data-ttu-id="704b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="704b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="704b8-105">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="704b8-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="704b8-106">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="704b8-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="704b8-107">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="704b8-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="704b8-108">方法</span><span class="sxs-lookup"><span data-stu-id="704b8-108">Methods</span></span>

| <span data-ttu-id="704b8-109">方法</span><span class="sxs-lookup"><span data-stu-id="704b8-109">Method</span></span>           | <span data-ttu-id="704b8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="704b8-110">Return Type</span></span>    |<span data-ttu-id="704b8-111">说明</span><span class="sxs-lookup"><span data-stu-id="704b8-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="704b8-112">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="704b8-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="704b8-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="704b8-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="704b8-114">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="704b8-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="704b8-115">List classes</span><span class="sxs-lookup"><span data-stu-id="704b8-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="704b8-116">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="704b8-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="704b8-117">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="704b8-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="704b8-118">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="704b8-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="704b8-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="704b8-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="704b8-120">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="704b8-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="704b8-121">List schools</span><span class="sxs-lookup"><span data-stu-id="704b8-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="704b8-122">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="704b8-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="704b8-123">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="704b8-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="704b8-124">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="704b8-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="704b8-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="704b8-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="704b8-126">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="704b8-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="704b8-127">List users</span><span class="sxs-lookup"><span data-stu-id="704b8-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="704b8-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="704b8-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="704b8-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="704b8-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="704b8-130">属性</span><span class="sxs-lookup"><span data-stu-id="704b8-130">Properties</span></span>
<span data-ttu-id="704b8-131">无。</span><span class="sxs-lookup"><span data-stu-id="704b8-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="704b8-132">关系</span><span class="sxs-lookup"><span data-stu-id="704b8-132">Relationships</span></span>
| <span data-ttu-id="704b8-133">关系</span><span class="sxs-lookup"><span data-stu-id="704b8-133">Relationship</span></span> | <span data-ttu-id="704b8-134">类型</span><span class="sxs-lookup"><span data-stu-id="704b8-134">Type</span></span>   |<span data-ttu-id="704b8-135">说明</span><span class="sxs-lookup"><span data-stu-id="704b8-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="704b8-136">classes</span><span class="sxs-lookup"><span data-stu-id="704b8-136">classes</span></span>|<span data-ttu-id="704b8-137">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="704b8-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="704b8-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="704b8-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="704b8-140">me</span><span class="sxs-lookup"><span data-stu-id="704b8-140">me</span></span>|[<span data-ttu-id="704b8-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="704b8-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="704b8-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="704b8-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="704b8-144">schools</span><span class="sxs-lookup"><span data-stu-id="704b8-144">schools</span></span>|<span data-ttu-id="704b8-145">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="704b8-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="704b8-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="704b8-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="704b8-148">users</span><span class="sxs-lookup"><span data-stu-id="704b8-148">users</span></span>|<span data-ttu-id="704b8-149">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="704b8-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="704b8-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="704b8-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="704b8-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="704b8-152">JSON representation</span></span>
<span data-ttu-id="704b8-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="704b8-153">Here is a JSON representation of the resource.</span></span>

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


# <a name="http"></a>[<span data-ttu-id="704b8-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="704b8-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="c"></a>[<span data-ttu-id="704b8-155">C#</span><span class="sxs-lookup"><span data-stu-id="704b8-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="704b8-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="704b8-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="704b8-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="704b8-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="704b8-158">Java</span><span class="sxs-lookup"><span data-stu-id="704b8-158">Java</span></span>](#tab/java)
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

