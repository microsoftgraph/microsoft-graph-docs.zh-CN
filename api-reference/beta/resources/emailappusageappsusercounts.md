---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d4dd1bc6a84b1d3e5f1b412986de686c9e6f5312
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979474"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="4752d-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="4752d-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="4752d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4752d-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="4752d-105">属性</span><span class="sxs-lookup"><span data-stu-id="4752d-105">Properties</span></span>

| <span data-ttu-id="4752d-106">属性</span><span class="sxs-lookup"><span data-stu-id="4752d-106">Property</span></span>          | <span data-ttu-id="4752d-107">类型</span><span class="sxs-lookup"><span data-stu-id="4752d-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="4752d-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4752d-108">reportRefreshDate</span></span> | <span data-ttu-id="4752d-109">日期</span><span class="sxs-lookup"><span data-stu-id="4752d-109">Date</span></span>   |
| <span data-ttu-id="4752d-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="4752d-110">mailForMac</span></span>        | <span data-ttu-id="4752d-111">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-111">Int64</span></span>  |
| <span data-ttu-id="4752d-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="4752d-112">outlookForMac</span></span>     | <span data-ttu-id="4752d-113">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-113">Int64</span></span>  |
| <span data-ttu-id="4752d-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="4752d-114">outlookForWindows</span></span> | <span data-ttu-id="4752d-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-115">Int64</span></span>  |
| <span data-ttu-id="4752d-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="4752d-116">outlookForMobile</span></span>  | <span data-ttu-id="4752d-117">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-117">Int64</span></span>  |
| <span data-ttu-id="4752d-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="4752d-118">otherForMobile</span></span>    | <span data-ttu-id="4752d-119">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-119">Int64</span></span>  |
| <span data-ttu-id="4752d-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="4752d-120">outlookForWeb</span></span>     | <span data-ttu-id="4752d-121">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-121">Int64</span></span>  |
| <span data-ttu-id="4752d-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="4752d-122">pop3App</span></span>           | <span data-ttu-id="4752d-123">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-123">Int64</span></span>  |
| <span data-ttu-id="4752d-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="4752d-124">imap4App</span></span>          | <span data-ttu-id="4752d-125">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-125">Int64</span></span>  |
| <span data-ttu-id="4752d-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="4752d-126">smtpApp</span></span>           | <span data-ttu-id="4752d-127">Int64</span><span class="sxs-lookup"><span data-stu-id="4752d-127">Int64</span></span>  |
| <span data-ttu-id="4752d-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4752d-128">reportPeriod</span></span>      | <span data-ttu-id="4752d-129">String</span><span class="sxs-lookup"><span data-stu-id="4752d-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4752d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4752d-130">JSON representation</span></span>

<span data-ttu-id="4752d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4752d-131">The following is a JSON representation of the resource.</span></span>

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


