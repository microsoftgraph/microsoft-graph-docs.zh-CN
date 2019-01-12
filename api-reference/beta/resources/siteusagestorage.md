---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928099"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="4c23e-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c23e-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4c23e-104">属性</span><span class="sxs-lookup"><span data-stu-id="4c23e-104">Properties</span></span>

| <span data-ttu-id="4c23e-105">属性</span><span class="sxs-lookup"><span data-stu-id="4c23e-105">Property</span></span>           | <span data-ttu-id="4c23e-106">类型</span><span class="sxs-lookup"><span data-stu-id="4c23e-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="4c23e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4c23e-107">reportRefreshDate</span></span>  | <span data-ttu-id="4c23e-108">日期</span><span class="sxs-lookup"><span data-stu-id="4c23e-108">Date</span></span>   |
| <span data-ttu-id="4c23e-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="4c23e-109">siteType</span></span>           | <span data-ttu-id="4c23e-110">字符串</span><span class="sxs-lookup"><span data-stu-id="4c23e-110">String</span></span> |
| <span data-ttu-id="4c23e-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4c23e-111">storageUsedInBytes</span></span> | <span data-ttu-id="4c23e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="4c23e-112">Int64</span></span>  |
| <span data-ttu-id="4c23e-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="4c23e-113">reportDate</span></span>         | <span data-ttu-id="4c23e-114">日期</span><span class="sxs-lookup"><span data-stu-id="4c23e-114">Date</span></span>   |
| <span data-ttu-id="4c23e-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4c23e-115">reportPeriod</span></span>       | <span data-ttu-id="4c23e-116">String</span><span class="sxs-lookup"><span data-stu-id="4c23e-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c23e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c23e-117">JSON representation</span></span>

<span data-ttu-id="4c23e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c23e-118">The following is a JSON representation of the resource.</span></span>

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
