---
title: teamsDeviceUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99cb675880962591d6298062f979f0930bc0a15d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964394"
---
# <a name="teamsdeviceusageusercounts-resource-type"></a><span data-ttu-id="965ea-103">teamsDeviceUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="965ea-103">teamsDeviceUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="965ea-104">属性</span><span class="sxs-lookup"><span data-stu-id="965ea-104">Properties</span></span>

| <span data-ttu-id="965ea-105">属性</span><span class="sxs-lookup"><span data-stu-id="965ea-105">Property</span></span>          | <span data-ttu-id="965ea-106">类型</span><span class="sxs-lookup"><span data-stu-id="965ea-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="965ea-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="965ea-107">reportRefreshDate</span></span> | <span data-ttu-id="965ea-108">日期</span><span class="sxs-lookup"><span data-stu-id="965ea-108">Date</span></span>   |
| <span data-ttu-id="965ea-109">web</span><span class="sxs-lookup"><span data-stu-id="965ea-109">web</span></span>               | <span data-ttu-id="965ea-110">Int64</span><span class="sxs-lookup"><span data-stu-id="965ea-110">Int64</span></span>  |
| <span data-ttu-id="965ea-111">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="965ea-111">windowsPhone</span></span>      | <span data-ttu-id="965ea-112">Int64</span><span class="sxs-lookup"><span data-stu-id="965ea-112">Int64</span></span>  |
| <span data-ttu-id="965ea-113">androidPhone</span><span class="sxs-lookup"><span data-stu-id="965ea-113">androidPhone</span></span>      | <span data-ttu-id="965ea-114">Int64</span><span class="sxs-lookup"><span data-stu-id="965ea-114">Int64</span></span>  |
| <span data-ttu-id="965ea-115">ios</span><span class="sxs-lookup"><span data-stu-id="965ea-115">ios</span></span>               | <span data-ttu-id="965ea-116">Int64</span><span class="sxs-lookup"><span data-stu-id="965ea-116">Int64</span></span>  |
| <span data-ttu-id="965ea-117">mac</span><span class="sxs-lookup"><span data-stu-id="965ea-117">mac</span></span>               | <span data-ttu-id="965ea-118">Int64</span><span class="sxs-lookup"><span data-stu-id="965ea-118">Int64</span></span>  |
| <span data-ttu-id="965ea-119">时间</span><span class="sxs-lookup"><span data-stu-id="965ea-119">windows</span></span>           | <span data-ttu-id="965ea-120">Int64</span><span class="sxs-lookup"><span data-stu-id="965ea-120">Int64</span></span>  |
| <span data-ttu-id="965ea-121">reportDate</span><span class="sxs-lookup"><span data-stu-id="965ea-121">reportDate</span></span>        | <span data-ttu-id="965ea-122">日期</span><span class="sxs-lookup"><span data-stu-id="965ea-122">Date</span></span>   |
| <span data-ttu-id="965ea-123">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="965ea-123">reportPeriod</span></span>      | <span data-ttu-id="965ea-124">String</span><span class="sxs-lookup"><span data-stu-id="965ea-124">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="965ea-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="965ea-125">JSON representation</span></span>

<span data-ttu-id="965ea-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="965ea-126">The following is a JSON representation of the resource.</span></span>

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
