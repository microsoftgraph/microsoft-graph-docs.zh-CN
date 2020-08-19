---
title: skypeForBusinessActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: a23c4d1aa4f548e4bc4ef1567b6f539ea749373a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811978"
---
# <a name="skypeforbusinessactivityusercounts-resource-type"></a><span data-ttu-id="188a3-103">skypeForBusinessActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="188a3-103">skypeForBusinessActivityUserCounts resource type</span></span>

<span data-ttu-id="188a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="188a3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="188a3-105">属性</span><span class="sxs-lookup"><span data-stu-id="188a3-105">Properties</span></span>

| <span data-ttu-id="188a3-106">属性</span><span class="sxs-lookup"><span data-stu-id="188a3-106">Property</span></span>          | <span data-ttu-id="188a3-107">类型</span><span class="sxs-lookup"><span data-stu-id="188a3-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="188a3-108">peerToPeer</span><span class="sxs-lookup"><span data-stu-id="188a3-108">peerToPeer</span></span>        | <span data-ttu-id="188a3-109">Int64</span><span class="sxs-lookup"><span data-stu-id="188a3-109">Int64</span></span>  |
| <span data-ttu-id="188a3-110">有条不紊</span><span class="sxs-lookup"><span data-stu-id="188a3-110">organized</span></span>         | <span data-ttu-id="188a3-111">Int64</span><span class="sxs-lookup"><span data-stu-id="188a3-111">Int64</span></span>  |
| <span data-ttu-id="188a3-112">参与</span><span class="sxs-lookup"><span data-stu-id="188a3-112">participated</span></span>      | <span data-ttu-id="188a3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="188a3-113">Int64</span></span>  |
| <span data-ttu-id="188a3-114">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="188a3-114">reportRefreshDate</span></span> | <span data-ttu-id="188a3-115">日期</span><span class="sxs-lookup"><span data-stu-id="188a3-115">Date</span></span>   |
| <span data-ttu-id="188a3-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="188a3-116">reportDate</span></span>        | <span data-ttu-id="188a3-117">日期</span><span class="sxs-lookup"><span data-stu-id="188a3-117">Date</span></span>   |
| <span data-ttu-id="188a3-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="188a3-118">reportPeriod</span></span>      | <span data-ttu-id="188a3-119">String</span><span class="sxs-lookup"><span data-stu-id="188a3-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="188a3-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="188a3-120">JSON representation</span></span>

<span data-ttu-id="188a3-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="188a3-121">The following is a JSON representation of the resource.</span></span>

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
