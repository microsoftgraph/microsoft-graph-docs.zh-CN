---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 98e387b97687a4aab55e8d94e72fdbfa585a0e84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042382"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="60ca6-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="60ca6-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="60ca6-104">属性</span><span class="sxs-lookup"><span data-stu-id="60ca6-104">Properties</span></span>

| <span data-ttu-id="60ca6-105">属性</span><span class="sxs-lookup"><span data-stu-id="60ca6-105">Property</span></span>          | <span data-ttu-id="60ca6-106">类型</span><span class="sxs-lookup"><span data-stu-id="60ca6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="60ca6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="60ca6-107">reportRefreshDate</span></span> | <span data-ttu-id="60ca6-108">日期</span><span class="sxs-lookup"><span data-stu-id="60ca6-108">Date</span></span>   |
| <span data-ttu-id="60ca6-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="60ca6-109">siteType</span></span>          | <span data-ttu-id="60ca6-110">字符串</span><span class="sxs-lookup"><span data-stu-id="60ca6-110">String</span></span> |
| <span data-ttu-id="60ca6-111">total</span><span class="sxs-lookup"><span data-stu-id="60ca6-111">total</span></span>             | <span data-ttu-id="60ca6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="60ca6-112">Int64</span></span>  |
| <span data-ttu-id="60ca6-113">活动</span><span class="sxs-lookup"><span data-stu-id="60ca6-113">active</span></span>            | <span data-ttu-id="60ca6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="60ca6-114">Int64</span></span>  |
| <span data-ttu-id="60ca6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="60ca6-115">reportDate</span></span>        | <span data-ttu-id="60ca6-116">日期</span><span class="sxs-lookup"><span data-stu-id="60ca6-116">Date</span></span>   |
| <span data-ttu-id="60ca6-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="60ca6-117">reportPeriod</span></span>      | <span data-ttu-id="60ca6-118">String</span><span class="sxs-lookup"><span data-stu-id="60ca6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="60ca6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60ca6-119">JSON representation</span></span>

<span data-ttu-id="60ca6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60ca6-120">The following is a JSON representation of the resource.</span></span>

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
