---
title: yammerGroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 9b997d111f31f290c0721172fdb59d9fdd0fd3bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518992"
---
# <a name="yammergroupsactivitycounts-resource-type"></a><span data-ttu-id="fcdcd-103">yammerGroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcdcd-103">yammerGroupsActivityCounts resource type</span></span>

<span data-ttu-id="fcdcd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcdcd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fcdcd-105">属性</span><span class="sxs-lookup"><span data-stu-id="fcdcd-105">Properties</span></span>

| <span data-ttu-id="fcdcd-106">属性</span><span class="sxs-lookup"><span data-stu-id="fcdcd-106">Property</span></span>          | <span data-ttu-id="fcdcd-107">类型</span><span class="sxs-lookup"><span data-stu-id="fcdcd-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fcdcd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fcdcd-108">reportRefreshDate</span></span> | <span data-ttu-id="fcdcd-109">日期</span><span class="sxs-lookup"><span data-stu-id="fcdcd-109">Date</span></span>   |
| <span data-ttu-id="fcdcd-110">人</span><span class="sxs-lookup"><span data-stu-id="fcdcd-110">liked</span></span>             | <span data-ttu-id="fcdcd-111">Int64</span><span class="sxs-lookup"><span data-stu-id="fcdcd-111">Int64</span></span>  |
| <span data-ttu-id="fcdcd-112">发布</span><span class="sxs-lookup"><span data-stu-id="fcdcd-112">posted</span></span>            | <span data-ttu-id="fcdcd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="fcdcd-113">Int64</span></span>  |
| <span data-ttu-id="fcdcd-114">自述</span><span class="sxs-lookup"><span data-stu-id="fcdcd-114">read</span></span>              | <span data-ttu-id="fcdcd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fcdcd-115">Int64</span></span>  |
| <span data-ttu-id="fcdcd-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="fcdcd-116">reportDate</span></span>        | <span data-ttu-id="fcdcd-117">日期</span><span class="sxs-lookup"><span data-stu-id="fcdcd-117">Date</span></span>   |
| <span data-ttu-id="fcdcd-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fcdcd-118">reportPeriod</span></span>      | <span data-ttu-id="fcdcd-119">String</span><span class="sxs-lookup"><span data-stu-id="fcdcd-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fcdcd-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcdcd-120">JSON representation</span></span>

<span data-ttu-id="fcdcd-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcdcd-121">The following is a JSON representation of the resource.</span></span>

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
