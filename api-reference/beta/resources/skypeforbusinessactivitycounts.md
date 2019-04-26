---
title: skypeForBusinessActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: e59bd33b1709780bac9726ee716ef9d81ef33c1f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568157"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="f5928-103">skypeForBusinessActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5928-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f5928-104">属性</span><span class="sxs-lookup"><span data-stu-id="f5928-104">Properties</span></span>

| <span data-ttu-id="f5928-105">属性</span><span class="sxs-lookup"><span data-stu-id="f5928-105">Property</span></span>          | <span data-ttu-id="f5928-106">类型</span><span class="sxs-lookup"><span data-stu-id="f5928-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f5928-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="f5928-107">peerToPeer</span></span>        | <span data-ttu-id="f5928-108">Int64</span><span class="sxs-lookup"><span data-stu-id="f5928-108">Int64</span></span>  |
| <span data-ttu-id="f5928-109">有条不紊</span><span class="sxs-lookup"><span data-stu-id="f5928-109">organized</span></span>         | <span data-ttu-id="f5928-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f5928-110">Int64</span></span>  |
| <span data-ttu-id="f5928-111">参与</span><span class="sxs-lookup"><span data-stu-id="f5928-111">participated</span></span>      | <span data-ttu-id="f5928-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f5928-112">Int64</span></span>  |
| <span data-ttu-id="f5928-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f5928-113">reportRefreshDate</span></span> | <span data-ttu-id="f5928-114">Date</span><span class="sxs-lookup"><span data-stu-id="f5928-114">Date</span></span>   |
| <span data-ttu-id="f5928-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="f5928-115">reportDate</span></span>        | <span data-ttu-id="f5928-116">Date</span><span class="sxs-lookup"><span data-stu-id="f5928-116">Date</span></span>   |
| <span data-ttu-id="f5928-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f5928-117">reportPeriod</span></span>      | <span data-ttu-id="f5928-118">String</span><span class="sxs-lookup"><span data-stu-id="f5928-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f5928-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5928-119">JSON representation</span></span>

<span data-ttu-id="f5928-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5928-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts"
} -->

```json
{
  "peerToPeer": 1024, 
  "organized": 1024, 
  "participated": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
