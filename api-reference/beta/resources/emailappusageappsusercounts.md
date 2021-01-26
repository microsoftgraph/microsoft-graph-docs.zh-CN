---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c6393d8f99d734c63c810622c91ce508adfecf23
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981828"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="fa041-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa041-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="fa041-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa041-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="fa041-105">属性</span><span class="sxs-lookup"><span data-stu-id="fa041-105">Properties</span></span>

| <span data-ttu-id="fa041-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa041-106">Property</span></span>          | <span data-ttu-id="fa041-107">类型</span><span class="sxs-lookup"><span data-stu-id="fa041-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="fa041-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fa041-108">reportRefreshDate</span></span> | <span data-ttu-id="fa041-109">日期</span><span class="sxs-lookup"><span data-stu-id="fa041-109">Date</span></span>   |
| <span data-ttu-id="fa041-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="fa041-110">mailForMac</span></span>        | <span data-ttu-id="fa041-111">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-111">Int64</span></span>  |
| <span data-ttu-id="fa041-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="fa041-112">outlookForMac</span></span>     | <span data-ttu-id="fa041-113">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-113">Int64</span></span>  |
| <span data-ttu-id="fa041-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="fa041-114">outlookForWindows</span></span> | <span data-ttu-id="fa041-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-115">Int64</span></span>  |
| <span data-ttu-id="fa041-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="fa041-116">outlookForMobile</span></span>  | <span data-ttu-id="fa041-117">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-117">Int64</span></span>  |
| <span data-ttu-id="fa041-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="fa041-118">otherForMobile</span></span>    | <span data-ttu-id="fa041-119">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-119">Int64</span></span>  |
| <span data-ttu-id="fa041-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="fa041-120">outlookForWeb</span></span>     | <span data-ttu-id="fa041-121">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-121">Int64</span></span>  |
| <span data-ttu-id="fa041-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="fa041-122">pop3App</span></span>           | <span data-ttu-id="fa041-123">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-123">Int64</span></span>  |
| <span data-ttu-id="fa041-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="fa041-124">imap4App</span></span>          | <span data-ttu-id="fa041-125">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-125">Int64</span></span>  |
| <span data-ttu-id="fa041-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="fa041-126">smtpApp</span></span>           | <span data-ttu-id="fa041-127">Int64</span><span class="sxs-lookup"><span data-stu-id="fa041-127">Int64</span></span>  |
| <span data-ttu-id="fa041-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fa041-128">reportPeriod</span></span>      | <span data-ttu-id="fa041-129">String</span><span class="sxs-lookup"><span data-stu-id="fa041-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa041-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa041-130">JSON representation</span></span>

<span data-ttu-id="fa041-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa041-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "mailForMac": 1024, 
  "outlookForMac": 1024, 
  "outlookForWindows": 1024, 
  "outlookForMobile": 1024, 
  "otherForMobile": 1024, 
  "outlookForWeb": 1024, 
  "pop3App": 1024, 
  "imap4App": 1024, 
  "smtpApp": 1024, 
  "reportPeriod": "String"
}
```


