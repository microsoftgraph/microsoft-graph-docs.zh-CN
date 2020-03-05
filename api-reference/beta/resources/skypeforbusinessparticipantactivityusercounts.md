---
title: skypeForBusinessParticipantActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a3a7ac37aeeb68d240ffa2c0cdec81e7b2d07ddc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520364"
---
# <a name="skypeforbusinessparticipantactivityusercounts-resource-type"></a><span data-ttu-id="52f02-103">skypeForBusinessParticipantActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="52f02-103">skypeForBusinessParticipantActivityUserCounts resource type</span></span>

<span data-ttu-id="52f02-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="52f02-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="52f02-105">属性</span><span class="sxs-lookup"><span data-stu-id="52f02-105">Properties</span></span>

| <span data-ttu-id="52f02-106">属性</span><span class="sxs-lookup"><span data-stu-id="52f02-106">Property</span></span>          | <span data-ttu-id="52f02-107">类型</span><span class="sxs-lookup"><span data-stu-id="52f02-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="52f02-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="52f02-108">im</span></span>                | <span data-ttu-id="52f02-109">Int64</span><span class="sxs-lookup"><span data-stu-id="52f02-109">Int64</span></span>  |
| <span data-ttu-id="52f02-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="52f02-110">audioVideo</span></span>        | <span data-ttu-id="52f02-111">Int64</span><span class="sxs-lookup"><span data-stu-id="52f02-111">Int64</span></span>  |
| <span data-ttu-id="52f02-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="52f02-112">appSharing</span></span>        | <span data-ttu-id="52f02-113">Int64</span><span class="sxs-lookup"><span data-stu-id="52f02-113">Int64</span></span>  |
| <span data-ttu-id="52f02-114">web</span><span class="sxs-lookup"><span data-stu-id="52f02-114">web</span></span>               | <span data-ttu-id="52f02-115">Int64</span><span class="sxs-lookup"><span data-stu-id="52f02-115">Int64</span></span>  |
| <span data-ttu-id="52f02-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="52f02-116">dialInOut3rdParty</span></span> | <span data-ttu-id="52f02-117">Int64</span><span class="sxs-lookup"><span data-stu-id="52f02-117">Int64</span></span>  |
| <span data-ttu-id="52f02-118">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="52f02-118">reportRefreshDate</span></span> | <span data-ttu-id="52f02-119">日期</span><span class="sxs-lookup"><span data-stu-id="52f02-119">Date</span></span>   |
| <span data-ttu-id="52f02-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="52f02-120">reportDate</span></span>        | <span data-ttu-id="52f02-121">日期</span><span class="sxs-lookup"><span data-stu-id="52f02-121">Date</span></span>   |
| <span data-ttu-id="52f02-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="52f02-122">reportPeriod</span></span>      | <span data-ttu-id="52f02-123">String</span><span class="sxs-lookup"><span data-stu-id="52f02-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="52f02-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52f02-124">JSON representation</span></span>

<span data-ttu-id="52f02-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52f02-125">The following is a JSON representation of the resource.</span></span>

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
