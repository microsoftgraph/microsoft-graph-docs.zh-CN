---
title: FilterCriteria 资源类型
description: 表示应用于列的筛选条件。
localization_priority: Normal
ms.openlocfilehash: 56663e802aacc2dab3f08462724d0994b5bada85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821677"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="af9fa-103">FilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="af9fa-103">FilterCriteria resource type</span></span>

> <span data-ttu-id="af9fa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="af9fa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af9fa-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="af9fa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="af9fa-106">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="af9fa-106">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af9fa-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af9fa-107">JSON representation</span></span>

<span data-ttu-id="af9fa-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af9fa-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```
