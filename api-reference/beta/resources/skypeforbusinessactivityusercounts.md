---
title: skypeForBusinessActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: e98133611d669a2a85bae65195fe70571d290442
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815482"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="8700f-103">skypeForBusinessActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="8700f-103">skypeForBusinessActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="8700f-104">属性</span><span class="sxs-lookup"><span data-stu-id="8700f-104">Properties</span></span>

| <span data-ttu-id="8700f-105">属性</span><span class="sxs-lookup"><span data-stu-id="8700f-105">Property</span></span>          | <span data-ttu-id="8700f-106">类型</span><span class="sxs-lookup"><span data-stu-id="8700f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="8700f-107">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="8700f-107">peerToPeer</span></span>        | <span data-ttu-id="8700f-108">Int64</span><span class="sxs-lookup"><span data-stu-id="8700f-108">Int64</span></span>  |
| <span data-ttu-id="8700f-109">组织</span><span class="sxs-lookup"><span data-stu-id="8700f-109">organized</span></span>         | <span data-ttu-id="8700f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="8700f-110">Int64</span></span>  |
| <span data-ttu-id="8700f-111">则参与了会议</span><span class="sxs-lookup"><span data-stu-id="8700f-111">participated</span></span>      | <span data-ttu-id="8700f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="8700f-112">Int64</span></span>  |
| <span data-ttu-id="8700f-113">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8700f-113">reportRefreshDate</span></span> | <span data-ttu-id="8700f-114">日期</span><span class="sxs-lookup"><span data-stu-id="8700f-114">Date</span></span>   |
| <span data-ttu-id="8700f-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="8700f-115">reportDate</span></span>        | <span data-ttu-id="8700f-116">日期</span><span class="sxs-lookup"><span data-stu-id="8700f-116">Date</span></span>   |
| <span data-ttu-id="8700f-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8700f-117">reportPeriod</span></span>      | <span data-ttu-id="8700f-118">String</span><span class="sxs-lookup"><span data-stu-id="8700f-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8700f-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8700f-119">JSON representation</span></span>

<span data-ttu-id="8700f-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8700f-120">The following is a JSON representation of the resource.</span></span>

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
