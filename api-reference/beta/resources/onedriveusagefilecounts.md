---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7e3a52d082d1acdd2e685008d60e6594615f57a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568101"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="e19ac-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e19ac-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e19ac-104">属性</span><span class="sxs-lookup"><span data-stu-id="e19ac-104">Properties</span></span>

| <span data-ttu-id="e19ac-105">属性</span><span class="sxs-lookup"><span data-stu-id="e19ac-105">Property</span></span>          | <span data-ttu-id="e19ac-106">类型</span><span class="sxs-lookup"><span data-stu-id="e19ac-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e19ac-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e19ac-107">reportRefreshDate</span></span> | <span data-ttu-id="e19ac-108">Date</span><span class="sxs-lookup"><span data-stu-id="e19ac-108">Date</span></span>   |
| <span data-ttu-id="e19ac-109">siteType</span><span class="sxs-lookup"><span data-stu-id="e19ac-109">siteType</span></span>          | <span data-ttu-id="e19ac-110">String</span><span class="sxs-lookup"><span data-stu-id="e19ac-110">String</span></span> |
| <span data-ttu-id="e19ac-111">total</span><span class="sxs-lookup"><span data-stu-id="e19ac-111">total</span></span>             | <span data-ttu-id="e19ac-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e19ac-112">Int64</span></span>  |
| <span data-ttu-id="e19ac-113">工作</span><span class="sxs-lookup"><span data-stu-id="e19ac-113">active</span></span>            | <span data-ttu-id="e19ac-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e19ac-114">Int64</span></span>  |
| <span data-ttu-id="e19ac-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="e19ac-115">reportDate</span></span>        | <span data-ttu-id="e19ac-116">Date</span><span class="sxs-lookup"><span data-stu-id="e19ac-116">Date</span></span>   |
| <span data-ttu-id="e19ac-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e19ac-117">reportPeriod</span></span>      | <span data-ttu-id="e19ac-118">String</span><span class="sxs-lookup"><span data-stu-id="e19ac-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e19ac-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e19ac-119">JSON representation</span></span>

<span data-ttu-id="e19ac-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e19ac-120">The following is a JSON representation of the resource.</span></span>

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
