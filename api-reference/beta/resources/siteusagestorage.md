---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 33d78540a6dd5b3c15cb6d8fce80496be19f0711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520518"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="42408-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="42408-103">siteUsageStorage resource type</span></span>

<span data-ttu-id="42408-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="42408-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="42408-105">属性</span><span class="sxs-lookup"><span data-stu-id="42408-105">Properties</span></span>

| <span data-ttu-id="42408-106">属性</span><span class="sxs-lookup"><span data-stu-id="42408-106">Property</span></span>           | <span data-ttu-id="42408-107">类型</span><span class="sxs-lookup"><span data-stu-id="42408-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="42408-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="42408-108">reportRefreshDate</span></span>  | <span data-ttu-id="42408-109">日期</span><span class="sxs-lookup"><span data-stu-id="42408-109">Date</span></span>   |
| <span data-ttu-id="42408-110">siteType</span><span class="sxs-lookup"><span data-stu-id="42408-110">siteType</span></span>           | <span data-ttu-id="42408-111">String</span><span class="sxs-lookup"><span data-stu-id="42408-111">String</span></span> |
| <span data-ttu-id="42408-112">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="42408-112">storageUsedInBytes</span></span> | <span data-ttu-id="42408-113">Int64</span><span class="sxs-lookup"><span data-stu-id="42408-113">Int64</span></span>  |
| <span data-ttu-id="42408-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="42408-114">reportDate</span></span>         | <span data-ttu-id="42408-115">日期</span><span class="sxs-lookup"><span data-stu-id="42408-115">Date</span></span>   |
| <span data-ttu-id="42408-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="42408-116">reportPeriod</span></span>       | <span data-ttu-id="42408-117">String</span><span class="sxs-lookup"><span data-stu-id="42408-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="42408-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42408-118">JSON representation</span></span>

<span data-ttu-id="42408-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42408-119">The following is a JSON representation of the resource.</span></span>

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
