---
title: 安全资源类型
description: 安全资源是安全对象模型的入口点。 它返回单一实例安全资源。 它不包含任何可用属性。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579210"
---
# <a name="security-resource-type"></a><span data-ttu-id="4aa67-105">安全资源类型</span><span class="sxs-lookup"><span data-stu-id="4aa67-105">security resource type</span></span>

<span data-ttu-id="4aa67-106">安全资源是安全对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="4aa67-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="4aa67-107">它返回单一实例安全资源。</span><span class="sxs-lookup"><span data-stu-id="4aa67-107">It returns a singleton security resource.</span></span> <span data-ttu-id="4aa67-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="4aa67-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="4aa67-109">方法</span><span class="sxs-lookup"><span data-stu-id="4aa67-109">Methods</span></span>

| <span data-ttu-id="4aa67-110">方法</span><span class="sxs-lookup"><span data-stu-id="4aa67-110">Method</span></span>       | <span data-ttu-id="4aa67-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="4aa67-111">Return Type</span></span> | <span data-ttu-id="4aa67-112">说明</span><span class="sxs-lookup"><span data-stu-id="4aa67-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4aa67-113">列出警报</span><span class="sxs-lookup"><span data-stu-id="4aa67-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="4aa67-114">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="4aa67-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="4aa67-115">获取一个警报对象集合。</span><span class="sxs-lookup"><span data-stu-id="4aa67-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="4aa67-116">获取通知</span><span class="sxs-lookup"><span data-stu-id="4aa67-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="4aa67-117">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="4aa67-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="4aa67-118">获取一个警报对象。</span><span class="sxs-lookup"><span data-stu-id="4aa67-118">Get a alert object.</span></span> |
| [<span data-ttu-id="4aa67-119">更新警报</span><span class="sxs-lookup"><span data-stu-id="4aa67-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="4aa67-120">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="4aa67-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="4aa67-121">获取一个警报对象。</span><span class="sxs-lookup"><span data-stu-id="4aa67-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4aa67-122">属性</span><span class="sxs-lookup"><span data-stu-id="4aa67-122">Properties</span></span>
<span data-ttu-id="4aa67-123">无</span><span class="sxs-lookup"><span data-stu-id="4aa67-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="4aa67-124">关系</span><span class="sxs-lookup"><span data-stu-id="4aa67-124">Relationships</span></span>
| <span data-ttu-id="4aa67-125">关系</span><span class="sxs-lookup"><span data-stu-id="4aa67-125">Relationship</span></span> | <span data-ttu-id="4aa67-126">类型</span><span class="sxs-lookup"><span data-stu-id="4aa67-126">Type</span></span>        | <span data-ttu-id="4aa67-127">说明</span><span class="sxs-lookup"><span data-stu-id="4aa67-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4aa67-128">警报</span><span class="sxs-lookup"><span data-stu-id="4aa67-128">alerts</span></span>|<span data-ttu-id="4aa67-129">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="4aa67-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="4aa67-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="4aa67-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="4aa67-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4aa67-132">JSON representation</span></span>
<span data-ttu-id="4aa67-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4aa67-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="4aa67-134">示例</span><span class="sxs-lookup"><span data-stu-id="4aa67-134">Example</span></span>

<span data-ttu-id="4aa67-135">**安全**资源在图形的根目录中可用。</span><span class="sxs-lookup"><span data-stu-id="4aa67-135">The **security** resource is available at the root of the graph.</span></span>

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
