---
title: teamsDeviceUsageUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ddfdef3e9d5500951fc24de5beb333e822c9bbda
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046452"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="41442-103">teamsDeviceUsageUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="41442-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="41442-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41442-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="41442-105">属性</span><span class="sxs-lookup"><span data-stu-id="41442-105">Properties</span></span>

| <span data-ttu-id="41442-106">属性</span><span class="sxs-lookup"><span data-stu-id="41442-106">Property</span></span>          | <span data-ttu-id="41442-107">类型</span><span class="sxs-lookup"><span data-stu-id="41442-107">Type</span></span>    |
| :---------------- | :------ |
| <span data-ttu-id="41442-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="41442-108">reportRefreshDate</span></span> | <span data-ttu-id="41442-109">日期</span><span class="sxs-lookup"><span data-stu-id="41442-109">Date</span></span>    |
| <span data-ttu-id="41442-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41442-110">userPrincipalName</span></span> | <span data-ttu-id="41442-111">String</span><span class="sxs-lookup"><span data-stu-id="41442-111">String</span></span>  |
| <span data-ttu-id="41442-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="41442-112">lastActivityDate</span></span>  | <span data-ttu-id="41442-113">日期</span><span class="sxs-lookup"><span data-stu-id="41442-113">Date</span></span>    |
| <span data-ttu-id="41442-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="41442-114">isDeleted</span></span>         | <span data-ttu-id="41442-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-115">Boolean</span></span> |
| <span data-ttu-id="41442-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="41442-116">deletedDate</span></span>       | <span data-ttu-id="41442-117">日期</span><span class="sxs-lookup"><span data-stu-id="41442-117">Date</span></span>    |
| <span data-ttu-id="41442-118">usedWeb</span><span class="sxs-lookup"><span data-stu-id="41442-118">usedWeb</span></span>           | <span data-ttu-id="41442-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-119">Boolean</span></span> |
| <span data-ttu-id="41442-120">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="41442-120">usedWindowsPhone</span></span>  | <span data-ttu-id="41442-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-121">Boolean</span></span> |
| <span data-ttu-id="41442-122">usediOS</span><span class="sxs-lookup"><span data-stu-id="41442-122">usediOS</span></span>           | <span data-ttu-id="41442-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-123">Boolean</span></span> |
| <span data-ttu-id="41442-124">usedMac</span><span class="sxs-lookup"><span data-stu-id="41442-124">usedMac</span></span>           | <span data-ttu-id="41442-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-125">Boolean</span></span> |
| <span data-ttu-id="41442-126">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="41442-126">usedAndroidPhone</span></span>  | <span data-ttu-id="41442-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-127">Boolean</span></span> |
| <span data-ttu-id="41442-128">usedWindows</span><span class="sxs-lookup"><span data-stu-id="41442-128">usedWindows</span></span>       | <span data-ttu-id="41442-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="41442-129">Boolean</span></span> |
| <span data-ttu-id="41442-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="41442-130">reportPeriod</span></span>      | <span data-ttu-id="41442-131">String</span><span class="sxs-lookup"><span data-stu-id="41442-131">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="41442-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41442-132">JSON representation</span></span>

<span data-ttu-id="41442-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41442-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "reportPeriod": "String"
}
```


