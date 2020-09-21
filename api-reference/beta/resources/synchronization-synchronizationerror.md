---
title: synchronizationError 资源类型
description: 表示同步过程中发生的错误。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7c32f3bc22d2357c0eca88e6f693cd958a6dd5ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013452"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="c9034-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9034-103">synchronizationError resource type</span></span>

<span data-ttu-id="c9034-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9034-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9034-105">表示同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="c9034-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="c9034-106">属性</span><span class="sxs-lookup"><span data-stu-id="c9034-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="c9034-107">属性</span><span class="sxs-lookup"><span data-stu-id="c9034-107">Property</span></span>     | <span data-ttu-id="c9034-108">类型</span><span class="sxs-lookup"><span data-stu-id="c9034-108">Type</span></span>   |<span data-ttu-id="c9034-109">说明</span><span class="sxs-lookup"><span data-stu-id="c9034-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9034-110">code</span><span class="sxs-lookup"><span data-stu-id="c9034-110">code</span></span>|<span data-ttu-id="c9034-111">String</span><span class="sxs-lookup"><span data-stu-id="c9034-111">String</span></span>||
|<span data-ttu-id="c9034-112">message</span><span class="sxs-lookup"><span data-stu-id="c9034-112">message</span></span>|<span data-ttu-id="c9034-113">String</span><span class="sxs-lookup"><span data-stu-id="c9034-113">String</span></span>||
|<span data-ttu-id="c9034-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="c9034-114">tenantActionable</span></span>|<span data-ttu-id="c9034-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9034-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="c9034-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9034-116">JSON representation</span></span>

<span data-ttu-id="c9034-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9034-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


