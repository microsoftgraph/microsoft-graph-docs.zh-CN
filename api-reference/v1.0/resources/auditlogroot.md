---
title: auditLogRoot 资源类型
description: 包含不同类型的审核日志。 此资源返回单一的 auditLog 资源。 它不包含任何可用属性。
author: dhanyahk
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 363d3a0c3aafbbd5b3d53914748dfdb1fd432b1b
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759725"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="72c84-105">auditLogRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="72c84-105">auditLogRoot resource type</span></span>

<span data-ttu-id="72c84-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72c84-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72c84-107">包含不同类型的审核日志。</span><span class="sxs-lookup"><span data-stu-id="72c84-107">Contains different types of audit logs.</span></span> <span data-ttu-id="72c84-108">此资源返回单一的 auditLog 资源。</span><span class="sxs-lookup"><span data-stu-id="72c84-108">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="72c84-109">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="72c84-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="72c84-110">方法</span><span class="sxs-lookup"><span data-stu-id="72c84-110">Methods</span></span>

| <span data-ttu-id="72c84-111">方法</span><span class="sxs-lookup"><span data-stu-id="72c84-111">Method</span></span>           | <span data-ttu-id="72c84-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="72c84-112">Return Type</span></span>    |<span data-ttu-id="72c84-113">说明</span><span class="sxs-lookup"><span data-stu-id="72c84-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72c84-114">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="72c84-114">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="72c84-115">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="72c84-115">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="72c84-116">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="72c84-116">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="72c84-117">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="72c84-117">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="72c84-118">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="72c84-118">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="72c84-119">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="72c84-119">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="72c84-120">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="72c84-120">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="72c84-121">signIn</span><span class="sxs-lookup"><span data-stu-id="72c84-121">signIn</span></span>](signin.md) |<span data-ttu-id="72c84-122">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72c84-122">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="72c84-123">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="72c84-123">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="72c84-124">signIn</span><span class="sxs-lookup"><span data-stu-id="72c84-124">signIn</span></span>](signin.md) |<span data-ttu-id="72c84-125">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="72c84-125">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="72c84-126">属性</span><span class="sxs-lookup"><span data-stu-id="72c84-126">Properties</span></span>

<span data-ttu-id="72c84-127">无。</span><span class="sxs-lookup"><span data-stu-id="72c84-127">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="72c84-128">关系</span><span class="sxs-lookup"><span data-stu-id="72c84-128">Relationships</span></span>

| <span data-ttu-id="72c84-129">关系</span><span class="sxs-lookup"><span data-stu-id="72c84-129">Relationship</span></span> | <span data-ttu-id="72c84-130">类型</span><span class="sxs-lookup"><span data-stu-id="72c84-130">Type</span></span>   |<span data-ttu-id="72c84-131">说明</span><span class="sxs-lookup"><span data-stu-id="72c84-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72c84-132">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="72c84-132">directoryAudits</span></span>|<span data-ttu-id="72c84-133">[directoryAudit](directoryaudit.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72c84-133">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="72c84-134">只读。</span><span class="sxs-lookup"><span data-stu-id="72c84-134">Read-only.</span></span> <span data-ttu-id="72c84-135">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="72c84-135">Nullable.</span></span>|
|<span data-ttu-id="72c84-136">signIns</span><span class="sxs-lookup"><span data-stu-id="72c84-136">signIns</span></span>|<span data-ttu-id="72c84-137">[signIn](signin.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72c84-137">[signIn](signin.md) collection</span></span>| <span data-ttu-id="72c84-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="72c84-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72c84-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72c84-140">JSON representation</span></span>

<span data-ttu-id="72c84-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72c84-141">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="72c84-142">示例</span><span class="sxs-lookup"><span data-stu-id="72c84-142">Example</span></span>


# <a name="http"></a>[<span data-ttu-id="72c84-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="72c84-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="c"></a>[<span data-ttu-id="72c84-144">C#</span><span class="sxs-lookup"><span data-stu-id="72c84-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="72c84-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72c84-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="72c84-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72c84-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="72c84-147">Java</span><span class="sxs-lookup"><span data-stu-id="72c84-147">Java</span></span>](#tab/java)
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

