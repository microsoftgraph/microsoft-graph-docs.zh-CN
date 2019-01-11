---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: ec428179cb35755e545aded70929eccd9d558fec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829531"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="940e8-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="940e8-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="940e8-104">属性</span><span class="sxs-lookup"><span data-stu-id="940e8-104">Properties</span></span>

| <span data-ttu-id="940e8-105">属性</span><span class="sxs-lookup"><span data-stu-id="940e8-105">Property</span></span>          | <span data-ttu-id="940e8-106">类型</span><span class="sxs-lookup"><span data-stu-id="940e8-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="940e8-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="940e8-107">reportRefreshDate</span></span> | <span data-ttu-id="940e8-108">日期</span><span class="sxs-lookup"><span data-stu-id="940e8-108">Date</span></span>   |
| <span data-ttu-id="940e8-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="940e8-109">siteType</span></span>          | <span data-ttu-id="940e8-110">字符串</span><span class="sxs-lookup"><span data-stu-id="940e8-110">String</span></span> |
| <span data-ttu-id="940e8-111">total</span><span class="sxs-lookup"><span data-stu-id="940e8-111">total</span></span>             | <span data-ttu-id="940e8-112">Int64</span><span class="sxs-lookup"><span data-stu-id="940e8-112">Int64</span></span>  |
| <span data-ttu-id="940e8-113">活动</span><span class="sxs-lookup"><span data-stu-id="940e8-113">active</span></span>            | <span data-ttu-id="940e8-114">Int64</span><span class="sxs-lookup"><span data-stu-id="940e8-114">Int64</span></span>  |
| <span data-ttu-id="940e8-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="940e8-115">reportDate</span></span>        | <span data-ttu-id="940e8-116">日期</span><span class="sxs-lookup"><span data-stu-id="940e8-116">Date</span></span>   |
| <span data-ttu-id="940e8-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="940e8-117">reportPeriod</span></span>      | <span data-ttu-id="940e8-118">String</span><span class="sxs-lookup"><span data-stu-id="940e8-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="940e8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="940e8-119">JSON representation</span></span>

<span data-ttu-id="940e8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="940e8-120">The following is a JSON representation of the resource.</span></span>

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
