---
title: skypeForBusinessOrganizerActivityUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: kszb
ms.openlocfilehash: f17f821b5234414185d359d98aa284233c1efb55
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808604"
---
# <a name="skypeforbusinessorganizeractivityusercounts-resource-type"></a><span data-ttu-id="45983-103">skypeForBusinessOrganizerActivityUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="45983-103">skypeForBusinessOrganizerActivityUserCounts resource type</span></span>

<span data-ttu-id="45983-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45983-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="45983-105">属性</span><span class="sxs-lookup"><span data-stu-id="45983-105">Properties</span></span>

| <span data-ttu-id="45983-106">属性</span><span class="sxs-lookup"><span data-stu-id="45983-106">Property</span></span>           | <span data-ttu-id="45983-107">类型</span><span class="sxs-lookup"><span data-stu-id="45983-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="45983-108">即时消息</span><span class="sxs-lookup"><span data-stu-id="45983-108">im</span></span>                 | <span data-ttu-id="45983-109">Int64</span><span class="sxs-lookup"><span data-stu-id="45983-109">Int64</span></span>  |
| <span data-ttu-id="45983-110">audioVideo</span><span class="sxs-lookup"><span data-stu-id="45983-110">audioVideo</span></span>         | <span data-ttu-id="45983-111">Int64</span><span class="sxs-lookup"><span data-stu-id="45983-111">Int64</span></span>  |
| <span data-ttu-id="45983-112">appSharing</span><span class="sxs-lookup"><span data-stu-id="45983-112">appSharing</span></span>         | <span data-ttu-id="45983-113">Int64</span><span class="sxs-lookup"><span data-stu-id="45983-113">Int64</span></span>  |
| <span data-ttu-id="45983-114">web</span><span class="sxs-lookup"><span data-stu-id="45983-114">web</span></span>                | <span data-ttu-id="45983-115">Int64</span><span class="sxs-lookup"><span data-stu-id="45983-115">Int64</span></span>  |
| <span data-ttu-id="45983-116">dialInOut3rdParty</span><span class="sxs-lookup"><span data-stu-id="45983-116">dialInOut3rdParty</span></span>  | <span data-ttu-id="45983-117">Int64</span><span class="sxs-lookup"><span data-stu-id="45983-117">Int64</span></span>  |
| <span data-ttu-id="45983-118">dialInOutMicrosoft</span><span class="sxs-lookup"><span data-stu-id="45983-118">dialInOutMicrosoft</span></span> | <span data-ttu-id="45983-119">Int64</span><span class="sxs-lookup"><span data-stu-id="45983-119">Int64</span></span>  |
| <span data-ttu-id="45983-120">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="45983-120">reportRefreshDate</span></span>  | <span data-ttu-id="45983-121">日期</span><span class="sxs-lookup"><span data-stu-id="45983-121">Date</span></span>   |
| <span data-ttu-id="45983-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="45983-122">reportDate</span></span>         | <span data-ttu-id="45983-123">日期</span><span class="sxs-lookup"><span data-stu-id="45983-123">Date</span></span>   |
| <span data-ttu-id="45983-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="45983-124">reportPeriod</span></span>       | <span data-ttu-id="45983-125">String</span><span class="sxs-lookup"><span data-stu-id="45983-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45983-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45983-126">JSON representation</span></span>

<span data-ttu-id="45983-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45983-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts"
} -->

```json
{
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
