---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: bf0b46c01167ac1d103b54386aabd981d99116cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009389"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="45b87-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="45b87-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="45b87-104">属性</span><span class="sxs-lookup"><span data-stu-id="45b87-104">Properties</span></span>

| <span data-ttu-id="45b87-105">属性</span><span class="sxs-lookup"><span data-stu-id="45b87-105">Property</span></span>          | <span data-ttu-id="45b87-106">类型</span><span class="sxs-lookup"><span data-stu-id="45b87-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="45b87-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="45b87-107">reportRefreshDate</span></span> | <span data-ttu-id="45b87-108">日期</span><span class="sxs-lookup"><span data-stu-id="45b87-108">Date</span></span>   |
| <span data-ttu-id="45b87-109">siteType</span><span class="sxs-lookup"><span data-stu-id="45b87-109">siteType</span></span>          | <span data-ttu-id="45b87-110">String</span><span class="sxs-lookup"><span data-stu-id="45b87-110">String</span></span> |
| <span data-ttu-id="45b87-111">total</span><span class="sxs-lookup"><span data-stu-id="45b87-111">total</span></span>             | <span data-ttu-id="45b87-112">Int64</span><span class="sxs-lookup"><span data-stu-id="45b87-112">Int64</span></span>  |
| <span data-ttu-id="45b87-113">工作</span><span class="sxs-lookup"><span data-stu-id="45b87-113">active</span></span>            | <span data-ttu-id="45b87-114">Int64</span><span class="sxs-lookup"><span data-stu-id="45b87-114">Int64</span></span>  |
| <span data-ttu-id="45b87-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="45b87-115">reportDate</span></span>        | <span data-ttu-id="45b87-116">日期</span><span class="sxs-lookup"><span data-stu-id="45b87-116">Date</span></span>   |
| <span data-ttu-id="45b87-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="45b87-117">reportPeriod</span></span>      | <span data-ttu-id="45b87-118">String</span><span class="sxs-lookup"><span data-stu-id="45b87-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45b87-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45b87-119">JSON representation</span></span>

<span data-ttu-id="45b87-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45b87-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
