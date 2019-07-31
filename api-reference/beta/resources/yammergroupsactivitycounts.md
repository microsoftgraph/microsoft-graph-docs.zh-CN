---
title: yammerGroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 12ab6de821ad4cd4362bcd3baa82525f6894b747
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963757"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="063e6-103">yammerGroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="063e6-103">yammerGroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="063e6-104">属性</span><span class="sxs-lookup"><span data-stu-id="063e6-104">Properties</span></span>

| <span data-ttu-id="063e6-105">属性</span><span class="sxs-lookup"><span data-stu-id="063e6-105">Property</span></span>          | <span data-ttu-id="063e6-106">类型</span><span class="sxs-lookup"><span data-stu-id="063e6-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="063e6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="063e6-107">reportRefreshDate</span></span> | <span data-ttu-id="063e6-108">日期</span><span class="sxs-lookup"><span data-stu-id="063e6-108">Date</span></span>   |
| <span data-ttu-id="063e6-109">人</span><span class="sxs-lookup"><span data-stu-id="063e6-109">liked</span></span>             | <span data-ttu-id="063e6-110">Int64</span><span class="sxs-lookup"><span data-stu-id="063e6-110">Int64</span></span>  |
| <span data-ttu-id="063e6-111">发布</span><span class="sxs-lookup"><span data-stu-id="063e6-111">posted</span></span>            | <span data-ttu-id="063e6-112">Int64</span><span class="sxs-lookup"><span data-stu-id="063e6-112">Int64</span></span>  |
| <span data-ttu-id="063e6-113">自述</span><span class="sxs-lookup"><span data-stu-id="063e6-113">read</span></span>              | <span data-ttu-id="063e6-114">Int64</span><span class="sxs-lookup"><span data-stu-id="063e6-114">Int64</span></span>  |
| <span data-ttu-id="063e6-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="063e6-115">reportDate</span></span>        | <span data-ttu-id="063e6-116">日期</span><span class="sxs-lookup"><span data-stu-id="063e6-116">Date</span></span>   |
| <span data-ttu-id="063e6-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="063e6-117">reportPeriod</span></span>      | <span data-ttu-id="063e6-118">String</span><span class="sxs-lookup"><span data-stu-id="063e6-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="063e6-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="063e6-119">JSON representation</span></span>

<span data-ttu-id="063e6-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="063e6-120">The following is a JSON representation of the resource.</span></span>

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
