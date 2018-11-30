---
title: skypeForBusinessActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 00c55df3a0a6201bd731938675880b9cbbe9cee6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047510"
---
# <a name="skypeforbusinessactivitycounts-resource-type"></a><span data-ttu-id="e2e9f-103">skypeForBusinessActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2e9f-103">skypeForBusinessActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e2e9f-104">属性</span><span class="sxs-lookup"><span data-stu-id="e2e9f-104">Properties</span></span>

| <span data-ttu-id="e2e9f-105">属性</span><span class="sxs-lookup"><span data-stu-id="e2e9f-105">Property</span></span>          | <span data-ttu-id="e2e9f-106">类型</span><span class="sxs-lookup"><span data-stu-id="e2e9f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="e2e9f-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="e2e9f-107">peerToPeer</span></span>        | <span data-ttu-id="e2e9f-108">Int64</span><span class="sxs-lookup"><span data-stu-id="e2e9f-108">Int64</span></span>  |
| <span data-ttu-id="e2e9f-109">组织</span><span class="sxs-lookup"><span data-stu-id="e2e9f-109">organized</span></span>         | <span data-ttu-id="e2e9f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e2e9f-110">Int64</span></span>  |
| <span data-ttu-id="e2e9f-111">则参与了会议</span><span class="sxs-lookup"><span data-stu-id="e2e9f-111">participated</span></span>      | <span data-ttu-id="e2e9f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e2e9f-112">Int64</span></span>  |
| <span data-ttu-id="e2e9f-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e2e9f-113">reportRefreshDate</span></span> | <span data-ttu-id="e2e9f-114">日期</span><span class="sxs-lookup"><span data-stu-id="e2e9f-114">Date</span></span>   |
| <span data-ttu-id="e2e9f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="e2e9f-115">reportDate</span></span>        | <span data-ttu-id="e2e9f-116">日期</span><span class="sxs-lookup"><span data-stu-id="e2e9f-116">Date</span></span>   |
| <span data-ttu-id="e2e9f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e2e9f-117">reportPeriod</span></span>      | <span data-ttu-id="e2e9f-118">String</span><span class="sxs-lookup"><span data-stu-id="e2e9f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2e9f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2e9f-119">JSON representation</span></span>

<span data-ttu-id="e2e9f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2e9f-120">The following is a JSON representation of the resource.</span></span>

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
