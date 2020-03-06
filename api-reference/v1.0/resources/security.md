---
title: 安全资源类型
description: 安全资源是安全对象模型的入口点。 它返回单一实例安全资源。 它不包含任何可用属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 89db6a8efbf50042e5514758ee5a7ae3b7f88de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533766"
---
# <a name="security-resource-type"></a><span data-ttu-id="fcdd5-105">安全资源类型</span><span class="sxs-lookup"><span data-stu-id="fcdd5-105">security resource type</span></span>

<span data-ttu-id="fcdd5-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcdd5-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcdd5-107">安全资源是安全对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-107">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="fcdd5-108">它返回单一实例安全资源。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-108">It returns a singleton security resource.</span></span> <span data-ttu-id="fcdd5-109">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-109">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="fcdd5-110">Methods</span><span class="sxs-lookup"><span data-stu-id="fcdd5-110">Methods</span></span>

| <span data-ttu-id="fcdd5-111">方法</span><span class="sxs-lookup"><span data-stu-id="fcdd5-111">Method</span></span>       | <span data-ttu-id="fcdd5-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="fcdd5-112">Return Type</span></span> | <span data-ttu-id="fcdd5-113">说明</span><span class="sxs-lookup"><span data-stu-id="fcdd5-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fcdd5-114">列出警报</span><span class="sxs-lookup"><span data-stu-id="fcdd5-114">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="fcdd5-115">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="fcdd5-115">[alert](alert.md) collection</span></span> | <span data-ttu-id="fcdd5-116">获取一个警报对象集合。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-116">Get a alert object collection.</span></span> |
| [<span data-ttu-id="fcdd5-117">获取通知</span><span class="sxs-lookup"><span data-stu-id="fcdd5-117">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="fcdd5-118">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="fcdd5-118">[alert](alert.md) collection</span></span> | <span data-ttu-id="fcdd5-119">获取一个警报对象。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-119">Get a alert object.</span></span> |
| [<span data-ttu-id="fcdd5-120">更新警报</span><span class="sxs-lookup"><span data-stu-id="fcdd5-120">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="fcdd5-121">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="fcdd5-121">[alert](alert.md) collection</span></span> | <span data-ttu-id="fcdd5-122">获取一个警报对象。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-122">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fcdd5-123">属性</span><span class="sxs-lookup"><span data-stu-id="fcdd5-123">Properties</span></span>
<span data-ttu-id="fcdd5-124">无</span><span class="sxs-lookup"><span data-stu-id="fcdd5-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fcdd5-125">关系</span><span class="sxs-lookup"><span data-stu-id="fcdd5-125">Relationships</span></span>
| <span data-ttu-id="fcdd5-126">关系</span><span class="sxs-lookup"><span data-stu-id="fcdd5-126">Relationship</span></span> | <span data-ttu-id="fcdd5-127">类型</span><span class="sxs-lookup"><span data-stu-id="fcdd5-127">Type</span></span>        | <span data-ttu-id="fcdd5-128">说明</span><span class="sxs-lookup"><span data-stu-id="fcdd5-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fcdd5-129">警报</span><span class="sxs-lookup"><span data-stu-id="fcdd5-129">alerts</span></span>|<span data-ttu-id="fcdd5-130">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="fcdd5-130">[alert](alert.md) collection</span></span>| <span data-ttu-id="fcdd5-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fcdd5-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcdd5-133">JSON representation</span></span>
<span data-ttu-id="fcdd5-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="fcdd5-135">示例</span><span class="sxs-lookup"><span data-stu-id="fcdd5-135">Example</span></span>

<span data-ttu-id="fcdd5-136">**安全**资源在图形的根目录中可用。</span><span class="sxs-lookup"><span data-stu-id="fcdd5-136">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
