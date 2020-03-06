---
title: educationRoot 资源类型
description: '`/education` 命名空间公开特定于教育部门的功能。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3792f0c867538c77522566110be36ac15d952396
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531548"
---
# <a name="educationroot-resource-type"></a><span data-ttu-id="388cd-103">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="388cd-103">educationRoot resource type</span></span>

<span data-ttu-id="388cd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="388cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="388cd-105">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="388cd-105">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="388cd-106">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="388cd-106">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="388cd-107">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="388cd-107">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="388cd-108">Methods</span><span class="sxs-lookup"><span data-stu-id="388cd-108">Methods</span></span>

| <span data-ttu-id="388cd-109">方法</span><span class="sxs-lookup"><span data-stu-id="388cd-109">Method</span></span>           | <span data-ttu-id="388cd-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="388cd-110">Return Type</span></span>    |<span data-ttu-id="388cd-111">说明</span><span class="sxs-lookup"><span data-stu-id="388cd-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="388cd-112">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="388cd-112">Create educationClass</span></span>](../api/educationroot-post-classes.md) |[<span data-ttu-id="388cd-113">educationClass</span><span class="sxs-lookup"><span data-stu-id="388cd-113">educationClass</span></span>](educationclass.md)| <span data-ttu-id="388cd-114">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="388cd-114">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="388cd-115">List classes</span><span class="sxs-lookup"><span data-stu-id="388cd-115">List classes</span></span>](../api/educationroot-list-classes.md) |<span data-ttu-id="388cd-116">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cd-116">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="388cd-117">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="388cd-117">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="388cd-118">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="388cd-118">Create educationSchool</span></span>](../api/educationroot-post-schools.md) |[<span data-ttu-id="388cd-119">educationSchool</span><span class="sxs-lookup"><span data-stu-id="388cd-119">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="388cd-120">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="388cd-120">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="388cd-121">List schools</span><span class="sxs-lookup"><span data-stu-id="388cd-121">List schools</span></span>](../api/educationroot-list-schools.md) |<span data-ttu-id="388cd-122">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cd-122">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="388cd-123">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="388cd-123">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="388cd-124">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="388cd-124">Create educationUser</span></span>](../api/educationroot-post-users.md) |[<span data-ttu-id="388cd-125">educationUser</span><span class="sxs-lookup"><span data-stu-id="388cd-125">educationUser</span></span>](educationuser.md)| <span data-ttu-id="388cd-126">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="388cd-126">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="388cd-127">List users</span><span class="sxs-lookup"><span data-stu-id="388cd-127">List users</span></span>](../api/educationroot-list-users.md) |<span data-ttu-id="388cd-128">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cd-128">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="388cd-129">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="388cd-129">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="388cd-130">属性</span><span class="sxs-lookup"><span data-stu-id="388cd-130">Properties</span></span>
<span data-ttu-id="388cd-131">无。</span><span class="sxs-lookup"><span data-stu-id="388cd-131">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="388cd-132">关系</span><span class="sxs-lookup"><span data-stu-id="388cd-132">Relationships</span></span>
| <span data-ttu-id="388cd-133">关系</span><span class="sxs-lookup"><span data-stu-id="388cd-133">Relationship</span></span> | <span data-ttu-id="388cd-134">类型</span><span class="sxs-lookup"><span data-stu-id="388cd-134">Type</span></span>   |<span data-ttu-id="388cd-135">说明</span><span class="sxs-lookup"><span data-stu-id="388cd-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="388cd-136">classes</span><span class="sxs-lookup"><span data-stu-id="388cd-136">classes</span></span>|<span data-ttu-id="388cd-137">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cd-137">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="388cd-138">只读。</span><span class="sxs-lookup"><span data-stu-id="388cd-138">Read-only.</span></span> <span data-ttu-id="388cd-139">可为空。</span><span class="sxs-lookup"><span data-stu-id="388cd-139">Nullable.</span></span>|
|<span data-ttu-id="388cd-140">me</span><span class="sxs-lookup"><span data-stu-id="388cd-140">me</span></span>|[<span data-ttu-id="388cd-141">educationUser</span><span class="sxs-lookup"><span data-stu-id="388cd-141">educationUser</span></span>](educationuser.md)| <span data-ttu-id="388cd-142">只读。</span><span class="sxs-lookup"><span data-stu-id="388cd-142">Read-only.</span></span> <span data-ttu-id="388cd-143">可为空。</span><span class="sxs-lookup"><span data-stu-id="388cd-143">Nullable.</span></span>|
|<span data-ttu-id="388cd-144">schools</span><span class="sxs-lookup"><span data-stu-id="388cd-144">schools</span></span>|<span data-ttu-id="388cd-145">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cd-145">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="388cd-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="388cd-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="388cd-148">users</span><span class="sxs-lookup"><span data-stu-id="388cd-148">users</span></span>|<span data-ttu-id="388cd-149">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="388cd-149">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="388cd-p105">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="388cd-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="388cd-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="388cd-152">JSON representation</span></span>
<span data-ttu-id="388cd-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="388cd-153">Here is a JSON representation of the resource.</span></span>

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


# <a name="http"></a>[<span data-ttu-id="388cd-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="388cd-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education
```
# <a name="c"></a>[<span data-ttu-id="388cd-155">C#</span><span class="sxs-lookup"><span data-stu-id="388cd-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-education-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="388cd-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="388cd-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-education-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="388cd-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="388cd-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-education-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="388cd-158">Java</span><span class="sxs-lookup"><span data-stu-id="388cd-158">Java</span></span>](#tab/java)
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
