---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 29f8e9b4ae1a559415bcd826aa1507836492d99a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979439"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="caf75-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="caf75-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="caf75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="caf75-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="caf75-105">属性</span><span class="sxs-lookup"><span data-stu-id="caf75-105">Properties</span></span>

| <span data-ttu-id="caf75-106">属性</span><span class="sxs-lookup"><span data-stu-id="caf75-106">Property</span></span>          | <span data-ttu-id="caf75-107">类型</span><span class="sxs-lookup"><span data-stu-id="caf75-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="caf75-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="caf75-108">reportRefreshDate</span></span> | <span data-ttu-id="caf75-109">日期</span><span class="sxs-lookup"><span data-stu-id="caf75-109">Date</span></span>   |
| <span data-ttu-id="caf75-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="caf75-110">mailForMac</span></span>        | <span data-ttu-id="caf75-111">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-111">Int64</span></span>  |
| <span data-ttu-id="caf75-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="caf75-112">outlookForMac</span></span>     | <span data-ttu-id="caf75-113">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-113">Int64</span></span>  |
| <span data-ttu-id="caf75-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="caf75-114">outlookForWindows</span></span> | <span data-ttu-id="caf75-115">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-115">Int64</span></span>  |
| <span data-ttu-id="caf75-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="caf75-116">outlookForMobile</span></span>  | <span data-ttu-id="caf75-117">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-117">Int64</span></span>  |
| <span data-ttu-id="caf75-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="caf75-118">otherForMobile</span></span>    | <span data-ttu-id="caf75-119">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-119">Int64</span></span>  |
| <span data-ttu-id="caf75-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="caf75-120">outlookForWeb</span></span>     | <span data-ttu-id="caf75-121">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-121">Int64</span></span>  |
| <span data-ttu-id="caf75-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="caf75-122">pop3App</span></span>           | <span data-ttu-id="caf75-123">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-123">Int64</span></span>  |
| <span data-ttu-id="caf75-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="caf75-124">imap4App</span></span>          | <span data-ttu-id="caf75-125">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-125">Int64</span></span>  |
| <span data-ttu-id="caf75-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="caf75-126">smtpApp</span></span>           | <span data-ttu-id="caf75-127">Int64</span><span class="sxs-lookup"><span data-stu-id="caf75-127">Int64</span></span>  |
| <span data-ttu-id="caf75-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="caf75-128">reportDate</span></span>        | <span data-ttu-id="caf75-129">日期</span><span class="sxs-lookup"><span data-stu-id="caf75-129">Date</span></span>   |
| <span data-ttu-id="caf75-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="caf75-130">reportPeriod</span></span>      | <span data-ttu-id="caf75-131">String</span><span class="sxs-lookup"><span data-stu-id="caf75-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="caf75-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="caf75-132">JSON representation</span></span>

<span data-ttu-id="caf75-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="caf75-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
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
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


