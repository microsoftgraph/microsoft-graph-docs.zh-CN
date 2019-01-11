---
title: synchronizationError 资源类型
description: 代表同步过程中发生的错误。
localization_priority: Normal
ms.openlocfilehash: cc6b58444ac56303bfd2e41f1fcae17658f6aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847241"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="28bbb-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="28bbb-103">synchronizationError resource type</span></span>

> <span data-ttu-id="28bbb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="28bbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28bbb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28bbb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28bbb-106">代表同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="28bbb-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="28bbb-107">属性</span><span class="sxs-lookup"><span data-stu-id="28bbb-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="28bbb-108">属性</span><span class="sxs-lookup"><span data-stu-id="28bbb-108">Property</span></span>     | <span data-ttu-id="28bbb-109">类型</span><span class="sxs-lookup"><span data-stu-id="28bbb-109">Type</span></span>   |<span data-ttu-id="28bbb-110">说明</span><span class="sxs-lookup"><span data-stu-id="28bbb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28bbb-111">code</span><span class="sxs-lookup"><span data-stu-id="28bbb-111">code</span></span>|<span data-ttu-id="28bbb-112">字符串</span><span class="sxs-lookup"><span data-stu-id="28bbb-112">String</span></span>||
|<span data-ttu-id="28bbb-113">message</span><span class="sxs-lookup"><span data-stu-id="28bbb-113">message</span></span>|<span data-ttu-id="28bbb-114">字符串</span><span class="sxs-lookup"><span data-stu-id="28bbb-114">String</span></span>||
|<span data-ttu-id="28bbb-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="28bbb-115">tenantActionable</span></span>|<span data-ttu-id="28bbb-116">布尔</span><span class="sxs-lookup"><span data-stu-id="28bbb-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="28bbb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28bbb-117">JSON representation</span></span>

<span data-ttu-id="28bbb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28bbb-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
