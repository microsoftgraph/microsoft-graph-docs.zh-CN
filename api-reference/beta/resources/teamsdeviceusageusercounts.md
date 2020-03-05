---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 02dc1b734e039e7c5eac7b8ffaed7a418e443c71
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519867"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="3d7ac-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d7ac-103">teamsDeviceUsageUserCounts resource type</span></span>

<span data-ttu-id="3d7ac-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3d7ac-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3d7ac-105">属性</span><span class="sxs-lookup"><span data-stu-id="3d7ac-105">Properties</span></span>

| <span data-ttu-id="3d7ac-106">属性</span><span class="sxs-lookup"><span data-stu-id="3d7ac-106">Property</span></span>          | <span data-ttu-id="3d7ac-107">类型</span><span class="sxs-lookup"><span data-stu-id="3d7ac-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="3d7ac-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3d7ac-108">reportRefreshDate</span></span> | <span data-ttu-id="3d7ac-109">日期</span><span class="sxs-lookup"><span data-stu-id="3d7ac-109">Date</span></span>   |
| <span data-ttu-id="3d7ac-110">web</span><span class="sxs-lookup"><span data-stu-id="3d7ac-110">web</span></span>               | <span data-ttu-id="3d7ac-111">Int64</span><span class="sxs-lookup"><span data-stu-id="3d7ac-111">Int64</span></span>  |
| <span data-ttu-id="3d7ac-112">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="3d7ac-112">windowsPhone</span></span>      | <span data-ttu-id="3d7ac-113">Int64</span><span class="sxs-lookup"><span data-stu-id="3d7ac-113">Int64</span></span>  |
| <span data-ttu-id="3d7ac-114">androidPhone</span><span class="sxs-lookup"><span data-stu-id="3d7ac-114">androidPhone</span></span>      | <span data-ttu-id="3d7ac-115">Int64</span><span class="sxs-lookup"><span data-stu-id="3d7ac-115">Int64</span></span>  |
| <span data-ttu-id="3d7ac-116">ios</span><span class="sxs-lookup"><span data-stu-id="3d7ac-116">ios</span></span>               | <span data-ttu-id="3d7ac-117">Int64</span><span class="sxs-lookup"><span data-stu-id="3d7ac-117">Int64</span></span>  |
| <span data-ttu-id="3d7ac-118">mac</span><span class="sxs-lookup"><span data-stu-id="3d7ac-118">mac</span></span>               | <span data-ttu-id="3d7ac-119">Int64</span><span class="sxs-lookup"><span data-stu-id="3d7ac-119">Int64</span></span>  |
| <span data-ttu-id="3d7ac-120">时间</span><span class="sxs-lookup"><span data-stu-id="3d7ac-120">windows</span></span>           | <span data-ttu-id="3d7ac-121">Int64</span><span class="sxs-lookup"><span data-stu-id="3d7ac-121">Int64</span></span>  |
| <span data-ttu-id="3d7ac-122">reportDate</span><span class="sxs-lookup"><span data-stu-id="3d7ac-122">reportDate</span></span>        | <span data-ttu-id="3d7ac-123">日期</span><span class="sxs-lookup"><span data-stu-id="3d7ac-123">Date</span></span>   |
| <span data-ttu-id="3d7ac-124">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3d7ac-124">reportPeriod</span></span>      | <span data-ttu-id="3d7ac-125">String</span><span class="sxs-lookup"><span data-stu-id="3d7ac-125">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3d7ac-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d7ac-126">JSON representation</span></span>

<span data-ttu-id="3d7ac-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d7ac-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "web": 1024, 
  "windowsPhone": 1024, 
  "androidPhone": 1024, 
  "ios": 1024, 
  "mac": 1024, 
  "windows": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
