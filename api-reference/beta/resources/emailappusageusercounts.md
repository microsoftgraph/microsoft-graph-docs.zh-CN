---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: a9878e2f98ca1beff51e6bd9ea803e8cbebeb390
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440553"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="5b727-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b727-103">emailAppUsageUserCounts resource type</span></span>

<span data-ttu-id="5b727-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b727-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5b727-105">属性</span><span class="sxs-lookup"><span data-stu-id="5b727-105">Properties</span></span>

| <span data-ttu-id="5b727-106">属性</span><span class="sxs-lookup"><span data-stu-id="5b727-106">Property</span></span>          | <span data-ttu-id="5b727-107">类型</span><span class="sxs-lookup"><span data-stu-id="5b727-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5b727-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5b727-108">reportRefreshDate</span></span> | <span data-ttu-id="5b727-109">日期</span><span class="sxs-lookup"><span data-stu-id="5b727-109">Date</span></span>   |
| <span data-ttu-id="5b727-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="5b727-110">mailForMac</span></span>        | <span data-ttu-id="5b727-111">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-111">Int64</span></span>  |
| <span data-ttu-id="5b727-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="5b727-112">outlookForMac</span></span>     | <span data-ttu-id="5b727-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-113">Int64</span></span>  |
| <span data-ttu-id="5b727-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="5b727-114">outlookForWindows</span></span> | <span data-ttu-id="5b727-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-115">Int64</span></span>  |
| <span data-ttu-id="5b727-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="5b727-116">outlookForMobile</span></span>  | <span data-ttu-id="5b727-117">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-117">Int64</span></span>  |
| <span data-ttu-id="5b727-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="5b727-118">otherForMobile</span></span>    | <span data-ttu-id="5b727-119">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-119">Int64</span></span>  |
| <span data-ttu-id="5b727-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="5b727-120">outlookForWeb</span></span>     | <span data-ttu-id="5b727-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-121">Int64</span></span>  |
| <span data-ttu-id="5b727-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="5b727-122">pop3App</span></span>           | <span data-ttu-id="5b727-123">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-123">Int64</span></span>  |
| <span data-ttu-id="5b727-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="5b727-124">imap4App</span></span>          | <span data-ttu-id="5b727-125">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-125">Int64</span></span>  |
| <span data-ttu-id="5b727-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="5b727-126">smtpApp</span></span>           | <span data-ttu-id="5b727-127">Int64</span><span class="sxs-lookup"><span data-stu-id="5b727-127">Int64</span></span>  |
| <span data-ttu-id="5b727-128">reportDate</span><span class="sxs-lookup"><span data-stu-id="5b727-128">reportDate</span></span>        | <span data-ttu-id="5b727-129">日期</span><span class="sxs-lookup"><span data-stu-id="5b727-129">Date</span></span>   |
| <span data-ttu-id="5b727-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5b727-130">reportPeriod</span></span>      | <span data-ttu-id="5b727-131">String</span><span class="sxs-lookup"><span data-stu-id="5b727-131">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5b727-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b727-132">JSON representation</span></span>

<span data-ttu-id="5b727-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b727-133">The following is a JSON representation of the resource.</span></span>

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
