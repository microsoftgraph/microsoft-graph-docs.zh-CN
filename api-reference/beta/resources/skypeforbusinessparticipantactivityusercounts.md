---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f6feb87de8b62dcf4f958a5c2bc6aaeda3ef454d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008108"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="5d870-103">skypeForBusinessParticipantActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d870-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5d870-104">属性</span><span class="sxs-lookup"><span data-stu-id="5d870-104">Properties</span></span>

| <span data-ttu-id="5d870-105">属性</span><span class="sxs-lookup"><span data-stu-id="5d870-105">Property</span></span>          | <span data-ttu-id="5d870-106">类型</span><span class="sxs-lookup"><span data-stu-id="5d870-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5d870-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="5d870-107">im</span></span>                | <span data-ttu-id="5d870-108">Int64</span><span class="sxs-lookup"><span data-stu-id="5d870-108">Int64</span></span>  |
| <span data-ttu-id="5d870-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="5d870-109">audioVideo</span></span>        | <span data-ttu-id="5d870-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5d870-110">Int64</span></span>  |
| <span data-ttu-id="5d870-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="5d870-111">appSharing</span></span>        | <span data-ttu-id="5d870-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5d870-112">Int64</span></span>  |
| <span data-ttu-id="5d870-113">web</span><span class="sxs-lookup"><span data-stu-id="5d870-113">web</span></span>               | <span data-ttu-id="5d870-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5d870-114">Int64</span></span>  |
| <span data-ttu-id="5d870-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="5d870-115">dialInOut3rdParty</span></span> | <span data-ttu-id="5d870-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5d870-116">Int64</span></span>  |
| <span data-ttu-id="5d870-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5d870-117">reportRefreshDate</span></span> | <span data-ttu-id="5d870-118">日期</span><span class="sxs-lookup"><span data-stu-id="5d870-118">Date</span></span>   |
| <span data-ttu-id="5d870-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="5d870-119">reportDate</span></span>        | <span data-ttu-id="5d870-120">日期</span><span class="sxs-lookup"><span data-stu-id="5d870-120">Date</span></span>   |
| <span data-ttu-id="5d870-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5d870-121">reportPeriod</span></span>      | <span data-ttu-id="5d870-122">String</span><span class="sxs-lookup"><span data-stu-id="5d870-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5d870-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d870-123">JSON representation</span></span>

<span data-ttu-id="5d870-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d870-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts"
} -->

```json
{
  "im": 1024, 
  "audioVideo": 196, 
  "appSharing": 196, 
  "web": 196, 
  "dialInOut3rdParty": 196, 
  "reportRefreshDate": "Date", 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
