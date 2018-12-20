---
title: callRoute 资源类型
description: CallRoute 类型。
author: VinodRavichandran
ms.openlocfilehash: 9538fb8f27f60e869c19edc7bd19d7f6b29e8fff
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380154"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="54aac-103">callRoute 资源类型</span><span class="sxs-lookup"><span data-stu-id="54aac-103">callRoute resource type</span></span>

> <span data-ttu-id="54aac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="54aac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54aac-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54aac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54aac-106">CallRoute 类型。</span><span class="sxs-lookup"><span data-stu-id="54aac-106">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="54aac-107">属性</span><span class="sxs-lookup"><span data-stu-id="54aac-107">Properties</span></span>

| <span data-ttu-id="54aac-108">属性</span><span class="sxs-lookup"><span data-stu-id="54aac-108">Property</span></span>            | <span data-ttu-id="54aac-109">类型</span><span class="sxs-lookup"><span data-stu-id="54aac-109">Type</span></span>                          | <span data-ttu-id="54aac-110">说明</span><span class="sxs-lookup"><span data-stu-id="54aac-110">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="54aac-111">最终</span><span class="sxs-lookup"><span data-stu-id="54aac-111">final</span></span>               | [<span data-ttu-id="54aac-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="54aac-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="54aac-113">解析为呼叫中的标识。</span><span class="sxs-lookup"><span data-stu-id="54aac-113">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="54aac-114">源语言</span><span class="sxs-lookup"><span data-stu-id="54aac-114">original</span></span>            | [<span data-ttu-id="54aac-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="54aac-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="54aac-116">最初在呼叫中使用的标识。</span><span class="sxs-lookup"><span data-stu-id="54aac-116">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="54aac-117">routingType</span><span class="sxs-lookup"><span data-stu-id="54aac-117">routingType</span></span>         | <span data-ttu-id="54aac-118">字符串</span><span class="sxs-lookup"><span data-stu-id="54aac-118">String</span></span>                        | <span data-ttu-id="54aac-119">可取值为：`forwarded`、`lookup`、`selfFork`。</span><span class="sxs-lookup"><span data-stu-id="54aac-119">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="54aac-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54aac-120">JSON representation</span></span>

<span data-ttu-id="54aac-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54aac-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
