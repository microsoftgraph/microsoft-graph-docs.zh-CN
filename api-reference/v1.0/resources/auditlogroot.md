---
title: auditLogRoot 资源类型
description: 包含不同类型的审核日志。 此资源返回 singleton auditLog 资源。 它不包含任何可用属性。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 204dfbb3f03be9550429694434bcb420b93e788d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951371"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="7e213-105">auditLogRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e213-105">auditLogRoot resource type</span></span>

<span data-ttu-id="7e213-106">包含不同类型的审核日志。</span><span class="sxs-lookup"><span data-stu-id="7e213-106">Contains different types of audit logs.</span></span> <span data-ttu-id="7e213-107">此资源返回 singleton auditLog 资源。</span><span class="sxs-lookup"><span data-stu-id="7e213-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="7e213-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="7e213-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="7e213-109">方法</span><span class="sxs-lookup"><span data-stu-id="7e213-109">Methods</span></span>

| <span data-ttu-id="7e213-110">方法</span><span class="sxs-lookup"><span data-stu-id="7e213-110">Method</span></span>           | <span data-ttu-id="7e213-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e213-111">Return Type</span></span>    |<span data-ttu-id="7e213-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e213-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7e213-113">列出 directoryAudits</span><span class="sxs-lookup"><span data-stu-id="7e213-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="7e213-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="7e213-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="7e213-115">列出集合中的目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="7e213-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="7e213-116">获取 directoryAudit</span><span class="sxs-lookup"><span data-stu-id="7e213-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="7e213-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="7e213-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="7e213-118">获取特定目录审核项及其属性。</span><span class="sxs-lookup"><span data-stu-id="7e213-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="7e213-119">列出 signIn</span><span class="sxs-lookup"><span data-stu-id="7e213-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="7e213-120">signIn</span><span class="sxs-lookup"><span data-stu-id="7e213-120">signIn</span></span>](signin.md) |<span data-ttu-id="7e213-121">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e213-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="7e213-122">获取 signIn</span><span class="sxs-lookup"><span data-stu-id="7e213-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="7e213-123">signIn</span><span class="sxs-lookup"><span data-stu-id="7e213-123">signIn</span></span>](signin.md) |<span data-ttu-id="7e213-124">读取 signIn 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e213-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e213-125">属性</span><span class="sxs-lookup"><span data-stu-id="7e213-125">Properties</span></span>

<span data-ttu-id="7e213-126">无。</span><span class="sxs-lookup"><span data-stu-id="7e213-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="7e213-127">关系</span><span class="sxs-lookup"><span data-stu-id="7e213-127">Relationships</span></span>

| <span data-ttu-id="7e213-128">关系</span><span class="sxs-lookup"><span data-stu-id="7e213-128">Relationship</span></span> | <span data-ttu-id="7e213-129">类型</span><span class="sxs-lookup"><span data-stu-id="7e213-129">Type</span></span>   |<span data-ttu-id="7e213-130">说明</span><span class="sxs-lookup"><span data-stu-id="7e213-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e213-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="7e213-131">directoryAudits</span></span>|<span data-ttu-id="7e213-132">[directoryAudit](directoryAudit.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e213-132">[directoryAudit](directoryAudit.md) collection</span></span>| <span data-ttu-id="7e213-133">只读。</span><span class="sxs-lookup"><span data-stu-id="7e213-133">Read-only.</span></span> <span data-ttu-id="7e213-134">可为空。</span><span class="sxs-lookup"><span data-stu-id="7e213-134">Nullable.</span></span>|
|<span data-ttu-id="7e213-135">signIns</span><span class="sxs-lookup"><span data-stu-id="7e213-135">signIns</span></span>|<span data-ttu-id="7e213-136">[登录](signIn.md)集合</span><span class="sxs-lookup"><span data-stu-id="7e213-136">[signIn](signIn.md) collection</span></span>| <span data-ttu-id="7e213-p104">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="7e213-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e213-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e213-139">JSON representation</span></span>

<span data-ttu-id="7e213-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e213-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="7e213-141">示例</span><span class="sxs-lookup"><span data-stu-id="7e213-141">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7e213-142">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7e213-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7e213-143">C#</span><span class="sxs-lookup"><span data-stu-id="7e213-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_auditLogs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e213-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e213-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_auditLogs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
