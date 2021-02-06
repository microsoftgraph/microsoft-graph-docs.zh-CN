---
title: synchronizationError 资源类型
description: 表示同步过程中发生的错误。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a49f2cf9b9d3e621533490127a5b2674ab43bf14
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131486"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="ee22a-103">synchronizationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee22a-103">synchronizationError resource type</span></span>

<span data-ttu-id="ee22a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee22a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee22a-105">表示同步过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="ee22a-105">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="ee22a-106">属性</span><span class="sxs-lookup"><span data-stu-id="ee22a-106">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="ee22a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee22a-107">Property</span></span>     | <span data-ttu-id="ee22a-108">类型</span><span class="sxs-lookup"><span data-stu-id="ee22a-108">Type</span></span>   |<span data-ttu-id="ee22a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ee22a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee22a-110">code</span><span class="sxs-lookup"><span data-stu-id="ee22a-110">code</span></span>|<span data-ttu-id="ee22a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="ee22a-111">String</span></span>||
|<span data-ttu-id="ee22a-112">message</span><span class="sxs-lookup"><span data-stu-id="ee22a-112">message</span></span>|<span data-ttu-id="ee22a-113">String</span><span class="sxs-lookup"><span data-stu-id="ee22a-113">String</span></span>||
|<span data-ttu-id="ee22a-114">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="ee22a-114">tenantActionable</span></span>|<span data-ttu-id="ee22a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee22a-115">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="ee22a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee22a-116">JSON representation</span></span>

<span data-ttu-id="ee22a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee22a-117">The following is a JSON representation of the resource.</span></span>

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


