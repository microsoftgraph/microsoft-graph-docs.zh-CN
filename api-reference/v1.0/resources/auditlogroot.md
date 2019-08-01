---
title: auditLogRoot 资源类型
description: 包含不同类型的审核日志。 此资源返回 singleton auditLog 资源。 它不包含任何可用属性。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2956b933b5d7703300964a0d6fd2014287f5e0ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030049"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="a8905-105">auditLogRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8905-105">auditLogRoot resource type</span></span>

<span data-ttu-id="a8905-106">包含不同类型的审核日志。</span><span class="sxs-lookup"><span data-stu-id="a8905-106">Contains different types of audit logs.</span></span> <span data-ttu-id="a8905-107">此资源返回 singleton auditLog 资源。</span><span class="sxs-lookup"><span data-stu-id="a8905-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="a8905-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="a8905-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a8905-109">方法</span><span class="sxs-lookup"><span data-stu-id="a8905-109">Methods</span></span>

| <span data-ttu-id="a8905-110">方法</span><span class="sxs-lookup"><span data-stu-id="a8905-110">Method</span></span>           | <span data-ttu-id="a8905-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8905-111">Return Type</span></span>    |<span data-ttu-id="a8905-112">说明</span><span class="sxs-lookup"><span data-stu-id="a8905-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8905-113">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="a8905-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="a8905-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="a8905-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="a8905-115">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="a8905-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="a8905-116">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="a8905-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="a8905-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="a8905-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="a8905-118">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="a8905-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="a8905-119">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="a8905-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="a8905-120">signIn</span><span class="sxs-lookup"><span data-stu-id="a8905-120">signIn</span></span>](signin.md) |<span data-ttu-id="a8905-121">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8905-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="a8905-122">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="a8905-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="a8905-123">signIn</span><span class="sxs-lookup"><span data-stu-id="a8905-123">signIn</span></span>](signin.md) |<span data-ttu-id="a8905-124">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8905-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8905-125">属性</span><span class="sxs-lookup"><span data-stu-id="a8905-125">Properties</span></span>

<span data-ttu-id="a8905-126">无。</span><span class="sxs-lookup"><span data-stu-id="a8905-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a8905-127">关系</span><span class="sxs-lookup"><span data-stu-id="a8905-127">Relationships</span></span>

| <span data-ttu-id="a8905-128">关系</span><span class="sxs-lookup"><span data-stu-id="a8905-128">Relationship</span></span> | <span data-ttu-id="a8905-129">类型</span><span class="sxs-lookup"><span data-stu-id="a8905-129">Type</span></span>   |<span data-ttu-id="a8905-130">说明</span><span class="sxs-lookup"><span data-stu-id="a8905-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8905-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="a8905-131">directoryAudits</span></span>|<span data-ttu-id="a8905-132">[directoryAudit](directoryaudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8905-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="a8905-133">只读。</span><span class="sxs-lookup"><span data-stu-id="a8905-133">Read-only.</span></span> <span data-ttu-id="a8905-134">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a8905-134">Nullable.</span></span>|
|<span data-ttu-id="a8905-135">signIns</span><span class="sxs-lookup"><span data-stu-id="a8905-135">signIns</span></span>|<span data-ttu-id="a8905-136">[登录](signin.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8905-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="a8905-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="a8905-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8905-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8905-139">JSON representation</span></span>

<span data-ttu-id="a8905-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8905-140">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="a8905-141">示例</span><span class="sxs-lookup"><span data-stu-id="a8905-141">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8905-142">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a8905-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8905-143">C#</span><span class="sxs-lookup"><span data-stu-id="a8905-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8905-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="a8905-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8905-145">目标-C</span><span class="sxs-lookup"><span data-stu-id="a8905-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a8905-146">Java</span><span class="sxs-lookup"><span data-stu-id="a8905-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditlogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
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
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
