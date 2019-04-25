---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c136b776e0c96a8bc63a1c82ae2ad17f059026cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583198"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="b3f57-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3f57-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b3f57-104">属性</span><span class="sxs-lookup"><span data-stu-id="b3f57-104">Properties</span></span>

| <span data-ttu-id="b3f57-105">属性</span><span class="sxs-lookup"><span data-stu-id="b3f57-105">Property</span></span>           | <span data-ttu-id="b3f57-106">类型</span><span class="sxs-lookup"><span data-stu-id="b3f57-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="b3f57-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b3f57-107">reportRefreshDate</span></span>  | <span data-ttu-id="b3f57-108">Date</span><span class="sxs-lookup"><span data-stu-id="b3f57-108">Date</span></span>   |
| <span data-ttu-id="b3f57-109">siteType</span><span class="sxs-lookup"><span data-stu-id="b3f57-109">siteType</span></span>           | <span data-ttu-id="b3f57-110">String</span><span class="sxs-lookup"><span data-stu-id="b3f57-110">String</span></span> |
| <span data-ttu-id="b3f57-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="b3f57-111">storageUsedInBytes</span></span> | <span data-ttu-id="b3f57-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b3f57-112">Int64</span></span>  |
| <span data-ttu-id="b3f57-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="b3f57-113">reportDate</span></span>         | <span data-ttu-id="b3f57-114">Date</span><span class="sxs-lookup"><span data-stu-id="b3f57-114">Date</span></span>   |
| <span data-ttu-id="b3f57-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b3f57-115">reportPeriod</span></span>       | <span data-ttu-id="b3f57-116">String</span><span class="sxs-lookup"><span data-stu-id="b3f57-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3f57-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3f57-117">JSON representation</span></span>

<span data-ttu-id="b3f57-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3f57-118">The following is a JSON representation of the resource.</span></span>

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
