---
title: yammerGroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: db9dfaa8c107acfa2c0f28fba2cfd06f242b166c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950828"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="de980-103">yammerGroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="de980-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="de980-104">属性</span><span class="sxs-lookup"><span data-stu-id="de980-104">Properties</span></span>

| <span data-ttu-id="de980-105">属性</span><span class="sxs-lookup"><span data-stu-id="de980-105">Property</span></span>          | <span data-ttu-id="de980-106">类型</span><span class="sxs-lookup"><span data-stu-id="de980-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="de980-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="de980-107">reportRefreshDate</span></span> | <span data-ttu-id="de980-108">日期</span><span class="sxs-lookup"><span data-stu-id="de980-108">Date</span></span>   |
| <span data-ttu-id="de980-109">满意</span><span class="sxs-lookup"><span data-stu-id="de980-109">liked</span></span>             | <span data-ttu-id="de980-110">Int64</span><span class="sxs-lookup"><span data-stu-id="de980-110">Int64</span></span>  |
| <span data-ttu-id="de980-111">发布</span><span class="sxs-lookup"><span data-stu-id="de980-111">posted</span></span>            | <span data-ttu-id="de980-112">Int64</span><span class="sxs-lookup"><span data-stu-id="de980-112">Int64</span></span>  |
| <span data-ttu-id="de980-113">读取</span><span class="sxs-lookup"><span data-stu-id="de980-113">read</span></span>              | <span data-ttu-id="de980-114">Int64</span><span class="sxs-lookup"><span data-stu-id="de980-114">Int64</span></span>  |
| <span data-ttu-id="de980-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="de980-115">reportDate</span></span>        | <span data-ttu-id="de980-116">日期</span><span class="sxs-lookup"><span data-stu-id="de980-116">Date</span></span>   |
| <span data-ttu-id="de980-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="de980-117">reportPeriod</span></span>      | <span data-ttu-id="de980-118">String</span><span class="sxs-lookup"><span data-stu-id="de980-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="de980-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de980-119">JSON representation</span></span>

<span data-ttu-id="de980-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de980-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "liked": 1024, 
  "posted": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
