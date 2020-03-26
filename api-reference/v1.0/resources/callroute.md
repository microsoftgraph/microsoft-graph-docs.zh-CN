---
title: callRoute 资源类型
description: 表示呼叫路由类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d316c6ba9a7a9d34b34110023019169c39859c79
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962522"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="da060-103">callRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="da060-103">callRoute resource type</span></span>

<span data-ttu-id="da060-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da060-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="da060-105">表示呼叫路由类型。</span><span class="sxs-lookup"><span data-stu-id="da060-105">Represents the call route type.</span></span>

## <a name="properties"></a><span data-ttu-id="da060-106">属性</span><span class="sxs-lookup"><span data-stu-id="da060-106">Properties</span></span>

| <span data-ttu-id="da060-107">属性</span><span class="sxs-lookup"><span data-stu-id="da060-107">Property</span></span>            | <span data-ttu-id="da060-108">类型</span><span class="sxs-lookup"><span data-stu-id="da060-108">Type</span></span>                          | <span data-ttu-id="da060-109">说明</span><span class="sxs-lookup"><span data-stu-id="da060-109">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="da060-110">终稿</span><span class="sxs-lookup"><span data-stu-id="da060-110">final</span></span>               | [<span data-ttu-id="da060-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="da060-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="da060-112">在呼叫中解析为的标识。</span><span class="sxs-lookup"><span data-stu-id="da060-112">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="da060-113">源语言</span><span class="sxs-lookup"><span data-stu-id="da060-113">original</span></span>            | [<span data-ttu-id="da060-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="da060-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="da060-115">最初在呼叫中使用的标识。</span><span class="sxs-lookup"><span data-stu-id="da060-115">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="da060-116">routingType</span><span class="sxs-lookup"><span data-stu-id="da060-116">routingType</span></span>         | <span data-ttu-id="da060-117">String</span><span class="sxs-lookup"><span data-stu-id="da060-117">String</span></span>                        | <span data-ttu-id="da060-118">可取值为：`forwarded`、`lookup`、`selfFork`。</span><span class="sxs-lookup"><span data-stu-id="da060-118">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="da060-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da060-119">JSON representation</span></span>

<span data-ttu-id="da060-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da060-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
