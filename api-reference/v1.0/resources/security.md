---
title: 安全资源类型
description: 安全资源是安全对象模型的入口点。 它返回 singleton 安全资源。 它不包含任何可用的属性。
ms.openlocfilehash: ddf00e46135733ef18c18918c0c365134138671f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008558"
---
# <a name="security-resource-type"></a><span data-ttu-id="b6f2c-105">安全资源类型</span><span class="sxs-lookup"><span data-stu-id="b6f2c-105">security resource type</span></span>

<span data-ttu-id="b6f2c-106">安全资源是安全对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="b6f2c-107">它返回 singleton 安全资源。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-107">It returns a singleton security resource.</span></span> <span data-ttu-id="b6f2c-108">它不包含任何可用的属性。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="b6f2c-109">方法</span><span class="sxs-lookup"><span data-stu-id="b6f2c-109">Methods</span></span>

| <span data-ttu-id="b6f2c-110">方法</span><span class="sxs-lookup"><span data-stu-id="b6f2c-110">Method</span></span>       | <span data-ttu-id="b6f2c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6f2c-111">Return Type</span></span> | <span data-ttu-id="b6f2c-112">说明</span><span class="sxs-lookup"><span data-stu-id="b6f2c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b6f2c-113">列出警报</span><span class="sxs-lookup"><span data-stu-id="b6f2c-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="b6f2c-114">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6f2c-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="b6f2c-115">获取通知对象集合。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="b6f2c-116">获取通知</span><span class="sxs-lookup"><span data-stu-id="b6f2c-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="b6f2c-117">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6f2c-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="b6f2c-118">获取通知对象。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-118">Get a alert object.</span></span> |
| [<span data-ttu-id="b6f2c-119">更新通知</span><span class="sxs-lookup"><span data-stu-id="b6f2c-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="b6f2c-120">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6f2c-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="b6f2c-121">获取通知对象。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6f2c-122">属性</span><span class="sxs-lookup"><span data-stu-id="b6f2c-122">Properties</span></span>
<span data-ttu-id="b6f2c-123">无</span><span class="sxs-lookup"><span data-stu-id="b6f2c-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="b6f2c-124">Relationships</span><span class="sxs-lookup"><span data-stu-id="b6f2c-124">Relationships</span></span>
| <span data-ttu-id="b6f2c-125">关系</span><span class="sxs-lookup"><span data-stu-id="b6f2c-125">Relationship</span></span> | <span data-ttu-id="b6f2c-126">类型</span><span class="sxs-lookup"><span data-stu-id="b6f2c-126">Type</span></span>        | <span data-ttu-id="b6f2c-127">说明</span><span class="sxs-lookup"><span data-stu-id="b6f2c-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6f2c-128">alerts</span><span class="sxs-lookup"><span data-stu-id="b6f2c-128">alerts</span></span>|<span data-ttu-id="b6f2c-129">[通知](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6f2c-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="b6f2c-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="b6f2c-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6f2c-132">JSON representation</span></span>
<span data-ttu-id="b6f2c-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="b6f2c-134">示例</span><span class="sxs-lookup"><span data-stu-id="b6f2c-134">Example</span></span>

<span data-ttu-id="b6f2c-135">可在图的根的**安全**资源。</span><span class="sxs-lookup"><span data-stu-id="b6f2c-135">The **security** resource is available at the root of the graph.</span></span>

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