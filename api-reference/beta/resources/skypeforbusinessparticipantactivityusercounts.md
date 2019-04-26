---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 6579552ef3ca5e9fefe8690a161bef4752ad2492
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568115"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="25942-103">skypeForBusinessParticipantActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="25942-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="25942-104">属性</span><span class="sxs-lookup"><span data-stu-id="25942-104">Properties</span></span>

| <span data-ttu-id="25942-105">属性</span><span class="sxs-lookup"><span data-stu-id="25942-105">Property</span></span>          | <span data-ttu-id="25942-106">类型</span><span class="sxs-lookup"><span data-stu-id="25942-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="25942-107">即时消息</span><span class="sxs-lookup"><span data-stu-id="25942-107">im</span></span>                | <span data-ttu-id="25942-108">Int64</span><span class="sxs-lookup"><span data-stu-id="25942-108">Int64</span></span>  |
| <span data-ttu-id="25942-109">audioVideo</span><span class="sxs-lookup"><span data-stu-id="25942-109">audioVideo</span></span>        | <span data-ttu-id="25942-110">Int64</span><span class="sxs-lookup"><span data-stu-id="25942-110">Int64</span></span>  |
| <span data-ttu-id="25942-111">appSharing</span><span class="sxs-lookup"><span data-stu-id="25942-111">appSharing</span></span>        | <span data-ttu-id="25942-112">Int64</span><span class="sxs-lookup"><span data-stu-id="25942-112">Int64</span></span>  |
| <span data-ttu-id="25942-113">web</span><span class="sxs-lookup"><span data-stu-id="25942-113">web</span></span>               | <span data-ttu-id="25942-114">Int64</span><span class="sxs-lookup"><span data-stu-id="25942-114">Int64</span></span>  |
| <span data-ttu-id="25942-115">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="25942-115">dialInOut3rdParty</span></span> | <span data-ttu-id="25942-116">Int64</span><span class="sxs-lookup"><span data-stu-id="25942-116">Int64</span></span>  |
| <span data-ttu-id="25942-117">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="25942-117">reportRefreshDate</span></span> | <span data-ttu-id="25942-118">Date</span><span class="sxs-lookup"><span data-stu-id="25942-118">Date</span></span>   |
| <span data-ttu-id="25942-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="25942-119">reportDate</span></span>        | <span data-ttu-id="25942-120">Date</span><span class="sxs-lookup"><span data-stu-id="25942-120">Date</span></span>   |
| <span data-ttu-id="25942-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="25942-121">reportPeriod</span></span>      | <span data-ttu-id="25942-122">String</span><span class="sxs-lookup"><span data-stu-id="25942-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25942-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25942-123">JSON representation</span></span>

<span data-ttu-id="25942-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25942-124">The following is a JSON representation of the resource.</span></span>

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
