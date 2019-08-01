---
title: 安全资源类型
description: 安全资源是安全对象模型的入口点。 它返回单一实例安全资源。 它不包含任何可用属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 87bd321a3c5e66cdc5d4fdc7fcb1407d02fbca1c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034452"
---
# <a name="security-resource-type"></a><span data-ttu-id="53425-105">安全资源类型</span><span class="sxs-lookup"><span data-stu-id="53425-105">security resource type</span></span>

<span data-ttu-id="53425-106">安全资源是安全对象模型的入口点。</span><span class="sxs-lookup"><span data-stu-id="53425-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="53425-107">它返回单一实例安全资源。</span><span class="sxs-lookup"><span data-stu-id="53425-107">It returns a singleton security resource.</span></span> <span data-ttu-id="53425-108">它不包含任何可用属性。</span><span class="sxs-lookup"><span data-stu-id="53425-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="53425-109">方法</span><span class="sxs-lookup"><span data-stu-id="53425-109">Methods</span></span>

| <span data-ttu-id="53425-110">方法</span><span class="sxs-lookup"><span data-stu-id="53425-110">Method</span></span>       | <span data-ttu-id="53425-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="53425-111">Return Type</span></span> | <span data-ttu-id="53425-112">说明</span><span class="sxs-lookup"><span data-stu-id="53425-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="53425-113">列出警报</span><span class="sxs-lookup"><span data-stu-id="53425-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="53425-114">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="53425-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="53425-115">获取一个警报对象集合。</span><span class="sxs-lookup"><span data-stu-id="53425-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="53425-116">获取通知</span><span class="sxs-lookup"><span data-stu-id="53425-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="53425-117">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="53425-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="53425-118">获取一个警报对象。</span><span class="sxs-lookup"><span data-stu-id="53425-118">Get a alert object.</span></span> |
| [<span data-ttu-id="53425-119">更新警报</span><span class="sxs-lookup"><span data-stu-id="53425-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="53425-120">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="53425-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="53425-121">获取一个警报对象。</span><span class="sxs-lookup"><span data-stu-id="53425-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="53425-122">属性</span><span class="sxs-lookup"><span data-stu-id="53425-122">Properties</span></span>
<span data-ttu-id="53425-123">无</span><span class="sxs-lookup"><span data-stu-id="53425-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="53425-124">关系</span><span class="sxs-lookup"><span data-stu-id="53425-124">Relationships</span></span>
| <span data-ttu-id="53425-125">关系</span><span class="sxs-lookup"><span data-stu-id="53425-125">Relationship</span></span> | <span data-ttu-id="53425-126">类型</span><span class="sxs-lookup"><span data-stu-id="53425-126">Type</span></span>        | <span data-ttu-id="53425-127">说明</span><span class="sxs-lookup"><span data-stu-id="53425-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53425-128">警报</span><span class="sxs-lookup"><span data-stu-id="53425-128">alerts</span></span>|<span data-ttu-id="53425-129">[警报](alert.md)集合</span><span class="sxs-lookup"><span data-stu-id="53425-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="53425-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="53425-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="53425-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53425-132">JSON representation</span></span>
<span data-ttu-id="53425-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53425-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="53425-134">示例</span><span class="sxs-lookup"><span data-stu-id="53425-134">Example</span></span>

<span data-ttu-id="53425-135">**安全**资源在图形的根目录中可用。</span><span class="sxs-lookup"><span data-stu-id="53425-135">The **security** resource is available at the root of the graph.</span></span>

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
