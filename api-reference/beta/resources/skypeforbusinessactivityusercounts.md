---
title: skypeForBusinessActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: eee736958540f2a3fb42cf3c76a37da4ebe78afd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049496"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="bdf48-103">skypeForBusinessActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdf48-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bdf48-104">属性</span><span class="sxs-lookup"><span data-stu-id="bdf48-104">Properties</span></span>

| <span data-ttu-id="bdf48-105">属性</span><span class="sxs-lookup"><span data-stu-id="bdf48-105">Property</span></span>          | <span data-ttu-id="bdf48-106">类型</span><span class="sxs-lookup"><span data-stu-id="bdf48-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="bdf48-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="bdf48-107">peerToPeer</span></span>        | <span data-ttu-id="bdf48-108">Int64</span><span class="sxs-lookup"><span data-stu-id="bdf48-108">Int64</span></span>  |
| <span data-ttu-id="bdf48-109">组织</span><span class="sxs-lookup"><span data-stu-id="bdf48-109">organized</span></span>         | <span data-ttu-id="bdf48-110">Int64</span><span class="sxs-lookup"><span data-stu-id="bdf48-110">Int64</span></span>  |
| <span data-ttu-id="bdf48-111">则参与了会议</span><span class="sxs-lookup"><span data-stu-id="bdf48-111">participated</span></span>      | <span data-ttu-id="bdf48-112">Int64</span><span class="sxs-lookup"><span data-stu-id="bdf48-112">Int64</span></span>  |
| <span data-ttu-id="bdf48-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bdf48-113">reportRefreshDate</span></span> | <span data-ttu-id="bdf48-114">日期</span><span class="sxs-lookup"><span data-stu-id="bdf48-114">Date</span></span>   |
| <span data-ttu-id="bdf48-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="bdf48-115">reportDate</span></span>        | <span data-ttu-id="bdf48-116">日期</span><span class="sxs-lookup"><span data-stu-id="bdf48-116">Date</span></span>   |
| <span data-ttu-id="bdf48-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bdf48-117">reportPeriod</span></span>      | <span data-ttu-id="bdf48-118">String</span><span class="sxs-lookup"><span data-stu-id="bdf48-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bdf48-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdf48-119">JSON representation</span></span>

<span data-ttu-id="bdf48-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdf48-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
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
