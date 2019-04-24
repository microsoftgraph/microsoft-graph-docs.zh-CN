---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506690"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="350b9-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="350b9-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="350b9-104">属性</span><span class="sxs-lookup"><span data-stu-id="350b9-104">Properties</span></span>

| <span data-ttu-id="350b9-105">属性</span><span class="sxs-lookup"><span data-stu-id="350b9-105">Property</span></span>          | <span data-ttu-id="350b9-106">类型</span><span class="sxs-lookup"><span data-stu-id="350b9-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="350b9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="350b9-107">reportRefreshDate</span></span> | <span data-ttu-id="350b9-108">Date</span><span class="sxs-lookup"><span data-stu-id="350b9-108">Date</span></span>   |
| <span data-ttu-id="350b9-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="350b9-109">mailForMac</span></span>        | <span data-ttu-id="350b9-110">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-110">Int64</span></span>  |
| <span data-ttu-id="350b9-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="350b9-111">outlookForMac</span></span>     | <span data-ttu-id="350b9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-112">Int64</span></span>  |
| <span data-ttu-id="350b9-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="350b9-113">outlookForWindows</span></span> | <span data-ttu-id="350b9-114">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-114">Int64</span></span>  |
| <span data-ttu-id="350b9-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="350b9-115">outlookForMobile</span></span>  | <span data-ttu-id="350b9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-116">Int64</span></span>  |
| <span data-ttu-id="350b9-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="350b9-117">otherForMobile</span></span>    | <span data-ttu-id="350b9-118">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-118">Int64</span></span>  |
| <span data-ttu-id="350b9-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="350b9-119">outlookForWeb</span></span>     | <span data-ttu-id="350b9-120">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-120">Int64</span></span>  |
| <span data-ttu-id="350b9-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="350b9-121">pop3App</span></span>           | <span data-ttu-id="350b9-122">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-122">Int64</span></span>  |
| <span data-ttu-id="350b9-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="350b9-123">imap4App</span></span>          | <span data-ttu-id="350b9-124">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-124">Int64</span></span>  |
| <span data-ttu-id="350b9-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="350b9-125">smtpApp</span></span>           | <span data-ttu-id="350b9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="350b9-126">Int64</span></span>  |
| <span data-ttu-id="350b9-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="350b9-127">reportDate</span></span>        | <span data-ttu-id="350b9-128">Date</span><span class="sxs-lookup"><span data-stu-id="350b9-128">Date</span></span>   |
| <span data-ttu-id="350b9-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="350b9-129">reportPeriod</span></span>      | <span data-ttu-id="350b9-130">字符串</span><span class="sxs-lookup"><span data-stu-id="350b9-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="350b9-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="350b9-131">JSON representation</span></span>

<span data-ttu-id="350b9-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="350b9-132">The following is a JSON representation of the resource.</span></span>

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
