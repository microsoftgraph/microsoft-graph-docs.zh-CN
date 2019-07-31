---
title: skypeForBusinessParticipantActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9e070dd3dc4687ee70f3189812e5f55ea90d718a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008122"
---
# <a name="skypeforbusinessparticipantactivitycounts-resource-type"></a><span data-ttu-id="70e00-103">skypeForBusinessParticipantActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="70e00-103">skypeForBusinessParticipantActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="70e00-104">属性</span><span class="sxs-lookup"><span data-stu-id="70e00-104">Properties</span></span>

| <span data-ttu-id="70e00-105">属性</span><span class="sxs-lookup"><span data-stu-id="70e00-105">Property</span></span>          | <span data-ttu-id="70e00-106">类型</span><span class="sxs-lookup"><span data-stu-id="70e00-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="70e00-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="70e00-107">im</span></span>                | <span data-ttu-id="70e00-108">Int64</span><span class="sxs-lookup"><span data-stu-id="70e00-108">Int64</span></span>  |
| <span data-ttu-id="70e00-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="70e00-109">audioVideo</span></span>        | <span data-ttu-id="70e00-110">Int64</span><span class="sxs-lookup"><span data-stu-id="70e00-110">Int64</span></span>  |
| <span data-ttu-id="70e00-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="70e00-111">appSharing</span></span>        | <span data-ttu-id="70e00-112">Int64</span><span class="sxs-lookup"><span data-stu-id="70e00-112">Int64</span></span>  |
| <span data-ttu-id="70e00-113">web</span><span class="sxs-lookup"><span data-stu-id="70e00-113">web</span></span>               | <span data-ttu-id="70e00-114">Int64</span><span class="sxs-lookup"><span data-stu-id="70e00-114">Int64</span></span>  |
| <span data-ttu-id="70e00-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="70e00-115">dialInOut3rdParty</span></span> | <span data-ttu-id="70e00-116">Int64</span><span class="sxs-lookup"><span data-stu-id="70e00-116">Int64</span></span>  |
| <span data-ttu-id="70e00-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="70e00-117">reportRefreshDate</span></span> | <span data-ttu-id="70e00-118">日期</span><span class="sxs-lookup"><span data-stu-id="70e00-118">Date</span></span>   |
| <span data-ttu-id="70e00-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="70e00-119">reportDate</span></span>        | <span data-ttu-id="70e00-120">日期</span><span class="sxs-lookup"><span data-stu-id="70e00-120">Date</span></span>   |
| <span data-ttu-id="70e00-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="70e00-121">reportPeriod</span></span>      | <span data-ttu-id="70e00-122">String</span><span class="sxs-lookup"><span data-stu-id="70e00-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70e00-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70e00-123">JSON representation</span></span>

<span data-ttu-id="70e00-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70e00-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 1024, 
  "appSharing": 1024, 
  "web": 1024, 
  "dialInOut3rdParty": 1024, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
