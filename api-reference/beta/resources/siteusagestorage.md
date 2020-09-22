---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 84b46861196e8893655fc5abc69ad1d4809cfd03
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033511"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="828e2-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="828e2-103">siteUsageStorage resource type</span></span>

<span data-ttu-id="828e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="828e2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="828e2-105">属性</span><span class="sxs-lookup"><span data-stu-id="828e2-105">Properties</span></span>

| <span data-ttu-id="828e2-106">属性</span><span class="sxs-lookup"><span data-stu-id="828e2-106">Property</span></span>           | <span data-ttu-id="828e2-107">类型</span><span class="sxs-lookup"><span data-stu-id="828e2-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="828e2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="828e2-108">reportRefreshDate</span></span>  | <span data-ttu-id="828e2-109">日期</span><span class="sxs-lookup"><span data-stu-id="828e2-109">Date</span></span>   |
| <span data-ttu-id="828e2-110">siteType</span><span class="sxs-lookup"><span data-stu-id="828e2-110">siteType</span></span>           | <span data-ttu-id="828e2-111">String</span><span class="sxs-lookup"><span data-stu-id="828e2-111">String</span></span> |
| <span data-ttu-id="828e2-112">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="828e2-112">storageUsedInBytes</span></span> | <span data-ttu-id="828e2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="828e2-113">Int64</span></span>  |
| <span data-ttu-id="828e2-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="828e2-114">reportDate</span></span>         | <span data-ttu-id="828e2-115">日期</span><span class="sxs-lookup"><span data-stu-id="828e2-115">Date</span></span>   |
| <span data-ttu-id="828e2-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="828e2-116">reportPeriod</span></span>       | <span data-ttu-id="828e2-117">String</span><span class="sxs-lookup"><span data-stu-id="828e2-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="828e2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="828e2-118">JSON representation</span></span>

<span data-ttu-id="828e2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="828e2-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "storageUsedInBytes": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


