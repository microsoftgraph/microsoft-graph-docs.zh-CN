---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 18ce0629bbb2a700d873587de6d3e5244304bcb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499489"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="d538e-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d538e-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="d538e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d538e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d538e-105">属性</span><span class="sxs-lookup"><span data-stu-id="d538e-105">Properties</span></span>

| <span data-ttu-id="d538e-106">属性</span><span class="sxs-lookup"><span data-stu-id="d538e-106">Property</span></span>          | <span data-ttu-id="d538e-107">类型</span><span class="sxs-lookup"><span data-stu-id="d538e-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="d538e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d538e-108">reportRefreshDate</span></span> | <span data-ttu-id="d538e-109">日期</span><span class="sxs-lookup"><span data-stu-id="d538e-109">Date</span></span>   |
| <span data-ttu-id="d538e-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="d538e-110">mailForMac</span></span>        | <span data-ttu-id="d538e-111">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-111">Int64</span></span>  |
| <span data-ttu-id="d538e-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="d538e-112">outlookForMac</span></span>     | <span data-ttu-id="d538e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-113">Int64</span></span>  |
| <span data-ttu-id="d538e-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="d538e-114">outlookForWindows</span></span> | <span data-ttu-id="d538e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-115">Int64</span></span>  |
| <span data-ttu-id="d538e-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="d538e-116">outlookForMobile</span></span>  | <span data-ttu-id="d538e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-117">Int64</span></span>  |
| <span data-ttu-id="d538e-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="d538e-118">otherForMobile</span></span>    | <span data-ttu-id="d538e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-119">Int64</span></span>  |
| <span data-ttu-id="d538e-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="d538e-120">outlookForWeb</span></span>     | <span data-ttu-id="d538e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-121">Int64</span></span>  |
| <span data-ttu-id="d538e-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="d538e-122">pop3App</span></span>           | <span data-ttu-id="d538e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-123">Int64</span></span>  |
| <span data-ttu-id="d538e-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="d538e-124">imap4App</span></span>          | <span data-ttu-id="d538e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-125">Int64</span></span>  |
| <span data-ttu-id="d538e-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="d538e-126">smtpApp</span></span>           | <span data-ttu-id="d538e-127">Int64</span><span class="sxs-lookup"><span data-stu-id="d538e-127">Int64</span></span>  |
| <span data-ttu-id="d538e-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="d538e-128">reportDate</span></span>        | <span data-ttu-id="d538e-129">日期</span><span class="sxs-lookup"><span data-stu-id="d538e-129">Date</span></span>   |
| <span data-ttu-id="d538e-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d538e-130">reportPeriod</span></span>      | <span data-ttu-id="d538e-131">String</span><span class="sxs-lookup"><span data-stu-id="d538e-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d538e-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d538e-132">JSON representation</span></span>

<span data-ttu-id="d538e-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d538e-133">The following is a JSON representation of the resource.</span></span>

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
