---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: a7e3a52d082d1acdd2e685008d60e6594615f57a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941021"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="b9088-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9088-103">oneDriveUsageFileCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b9088-104">属性</span><span class="sxs-lookup"><span data-stu-id="b9088-104">Properties</span></span>

| <span data-ttu-id="b9088-105">属性</span><span class="sxs-lookup"><span data-stu-id="b9088-105">Property</span></span>          | <span data-ttu-id="b9088-106">类型</span><span class="sxs-lookup"><span data-stu-id="b9088-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b9088-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b9088-107">reportRefreshDate</span></span> | <span data-ttu-id="b9088-108">日期</span><span class="sxs-lookup"><span data-stu-id="b9088-108">Date</span></span>   |
| <span data-ttu-id="b9088-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="b9088-109">siteType</span></span>          | <span data-ttu-id="b9088-110">字符串</span><span class="sxs-lookup"><span data-stu-id="b9088-110">String</span></span> |
| <span data-ttu-id="b9088-111">total</span><span class="sxs-lookup"><span data-stu-id="b9088-111">total</span></span>             | <span data-ttu-id="b9088-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b9088-112">Int64</span></span>  |
| <span data-ttu-id="b9088-113">活动</span><span class="sxs-lookup"><span data-stu-id="b9088-113">active</span></span>            | <span data-ttu-id="b9088-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b9088-114">Int64</span></span>  |
| <span data-ttu-id="b9088-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="b9088-115">reportDate</span></span>        | <span data-ttu-id="b9088-116">日期</span><span class="sxs-lookup"><span data-stu-id="b9088-116">Date</span></span>   |
| <span data-ttu-id="b9088-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b9088-117">reportPeriod</span></span>      | <span data-ttu-id="b9088-118">String</span><span class="sxs-lookup"><span data-stu-id="b9088-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9088-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9088-119">JSON representation</span></span>

<span data-ttu-id="b9088-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9088-120">The following is a JSON representation of the resource.</span></span>

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
