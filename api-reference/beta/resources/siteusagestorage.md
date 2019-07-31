---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 1ed15d4efb1c9a0fa81fdd79faeb9542d8093aab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008227"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="31f84-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="31f84-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="31f84-104">属性</span><span class="sxs-lookup"><span data-stu-id="31f84-104">Properties</span></span>

| <span data-ttu-id="31f84-105">属性</span><span class="sxs-lookup"><span data-stu-id="31f84-105">Property</span></span>           | <span data-ttu-id="31f84-106">类型</span><span class="sxs-lookup"><span data-stu-id="31f84-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="31f84-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="31f84-107">reportRefreshDate</span></span>  | <span data-ttu-id="31f84-108">日期</span><span class="sxs-lookup"><span data-stu-id="31f84-108">Date</span></span>   |
| <span data-ttu-id="31f84-109">siteType</span><span class="sxs-lookup"><span data-stu-id="31f84-109">siteType</span></span>           | <span data-ttu-id="31f84-110">String</span><span class="sxs-lookup"><span data-stu-id="31f84-110">String</span></span> |
| <span data-ttu-id="31f84-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="31f84-111">storageUsedInBytes</span></span> | <span data-ttu-id="31f84-112">Int64</span><span class="sxs-lookup"><span data-stu-id="31f84-112">Int64</span></span>  |
| <span data-ttu-id="31f84-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="31f84-113">reportDate</span></span>         | <span data-ttu-id="31f84-114">日期</span><span class="sxs-lookup"><span data-stu-id="31f84-114">Date</span></span>   |
| <span data-ttu-id="31f84-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="31f84-115">reportPeriod</span></span>       | <span data-ttu-id="31f84-116">String</span><span class="sxs-lookup"><span data-stu-id="31f84-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31f84-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31f84-117">JSON representation</span></span>

<span data-ttu-id="31f84-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31f84-118">The following is a JSON representation of the resource.</span></span>

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
