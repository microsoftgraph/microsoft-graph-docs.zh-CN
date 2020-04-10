---
title: synchronizationError 资源类型
description: 表示同步过程中发生的错误。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 884c39273d8d474a228cd8f4a8f2b321950e8caf
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217547"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="aec0d-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="aec0d-103">synchronizationError resource type</span></span>

<span data-ttu-id="aec0d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aec0d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aec0d-105">表示同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="aec0d-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="aec0d-106">属性</span><span class="sxs-lookup"><span data-stu-id="aec0d-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="aec0d-107">属性</span><span class="sxs-lookup"><span data-stu-id="aec0d-107">Property</span></span>     | <span data-ttu-id="aec0d-108">类型</span><span class="sxs-lookup"><span data-stu-id="aec0d-108">Type</span></span>   |<span data-ttu-id="aec0d-109">说明</span><span class="sxs-lookup"><span data-stu-id="aec0d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aec0d-110">code</span><span class="sxs-lookup"><span data-stu-id="aec0d-110">code</span></span>|<span data-ttu-id="aec0d-111">字符串</span><span class="sxs-lookup"><span data-stu-id="aec0d-111">String</span></span>||
|<span data-ttu-id="aec0d-112">message</span><span class="sxs-lookup"><span data-stu-id="aec0d-112">message</span></span>|<span data-ttu-id="aec0d-113">String</span><span class="sxs-lookup"><span data-stu-id="aec0d-113">String</span></span>||
|<span data-ttu-id="aec0d-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="aec0d-114">tenantActionable</span></span>|<span data-ttu-id="aec0d-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="aec0d-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="aec0d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aec0d-116">JSON representation</span></span>

<span data-ttu-id="aec0d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aec0d-117">The following is a JSON representation of the resource.</span></span>

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
