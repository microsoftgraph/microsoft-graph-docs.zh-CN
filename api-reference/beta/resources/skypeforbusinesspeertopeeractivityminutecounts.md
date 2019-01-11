---
title: skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 695c2fc57ab9d105b2576a9228ccc58d74b0094d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851616"
---
# <a name="skypeforbusinesspeertopeeractivityminutecounts-resource-type"></a><span data-ttu-id="62717-103">skypeForBusinessPeerToPeerActivityMinuteCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="62717-103">skypeForBusinessPeerToPeerActivityMinuteCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="62717-104">属性</span><span class="sxs-lookup"><span data-stu-id="62717-104">Properties</span></span>

| <span data-ttu-id="62717-105">属性</span><span class="sxs-lookup"><span data-stu-id="62717-105">Property</span></span>          | <span data-ttu-id="62717-106">类型</span><span class="sxs-lookup"><span data-stu-id="62717-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="62717-107">audio</span><span class="sxs-lookup"><span data-stu-id="62717-107">audio</span></span>             | <span data-ttu-id="62717-108">Int64</span><span class="sxs-lookup"><span data-stu-id="62717-108">Int64</span></span>  |
| <span data-ttu-id="62717-109">video</span><span class="sxs-lookup"><span data-stu-id="62717-109">video</span></span>             | <span data-ttu-id="62717-110">Int64</span><span class="sxs-lookup"><span data-stu-id="62717-110">Int64</span></span>  |
| <span data-ttu-id="62717-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="62717-111">reportRefreshDate</span></span> | <span data-ttu-id="62717-112">日期</span><span class="sxs-lookup"><span data-stu-id="62717-112">Date</span></span>   |
| <span data-ttu-id="62717-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="62717-113">reportDate</span></span>        | <span data-ttu-id="62717-114">日期</span><span class="sxs-lookup"><span data-stu-id="62717-114">Date</span></span>   |
| <span data-ttu-id="62717-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="62717-115">reportPeriod</span></span>      | <span data-ttu-id="62717-116">String</span><span class="sxs-lookup"><span data-stu-id="62717-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="62717-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62717-117">JSON representation</span></span>

<span data-ttu-id="62717-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62717-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts"
} -->

```json
{
  "audio": 1024, 
  "video": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
