---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7822528aacc9d6f104012d43004fbb9aabba127c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990801"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="f4dcc-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4dcc-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f4dcc-104">属性</span><span class="sxs-lookup"><span data-stu-id="f4dcc-104">Properties</span></span>

| <span data-ttu-id="f4dcc-105">属性</span><span class="sxs-lookup"><span data-stu-id="f4dcc-105">Property</span></span>          | <span data-ttu-id="f4dcc-106">类型</span><span class="sxs-lookup"><span data-stu-id="f4dcc-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f4dcc-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f4dcc-107">reportRefreshDate</span></span> | <span data-ttu-id="f4dcc-108">日期</span><span class="sxs-lookup"><span data-stu-id="f4dcc-108">Date</span></span>   |
| <span data-ttu-id="f4dcc-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="f4dcc-109">mailForMac</span></span>        | <span data-ttu-id="f4dcc-110">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-110">Int64</span></span>  |
| <span data-ttu-id="f4dcc-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="f4dcc-111">outlookForMac</span></span>     | <span data-ttu-id="f4dcc-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-112">Int64</span></span>  |
| <span data-ttu-id="f4dcc-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="f4dcc-113">outlookForWindows</span></span> | <span data-ttu-id="f4dcc-114">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-114">Int64</span></span>  |
| <span data-ttu-id="f4dcc-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="f4dcc-115">outlookForMobile</span></span>  | <span data-ttu-id="f4dcc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-116">Int64</span></span>  |
| <span data-ttu-id="f4dcc-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="f4dcc-117">otherForMobile</span></span>    | <span data-ttu-id="f4dcc-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-118">Int64</span></span>  |
| <span data-ttu-id="f4dcc-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="f4dcc-119">outlookForWeb</span></span>     | <span data-ttu-id="f4dcc-120">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-120">Int64</span></span>  |
| <span data-ttu-id="f4dcc-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="f4dcc-121">pop3App</span></span>           | <span data-ttu-id="f4dcc-122">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-122">Int64</span></span>  |
| <span data-ttu-id="f4dcc-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="f4dcc-123">imap4App</span></span>          | <span data-ttu-id="f4dcc-124">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-124">Int64</span></span>  |
| <span data-ttu-id="f4dcc-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="f4dcc-125">smtpApp</span></span>           | <span data-ttu-id="f4dcc-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f4dcc-126">Int64</span></span>  |
| <span data-ttu-id="f4dcc-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="f4dcc-127">reportDate</span></span>        | <span data-ttu-id="f4dcc-128">日期</span><span class="sxs-lookup"><span data-stu-id="f4dcc-128">Date</span></span>   |
| <span data-ttu-id="f4dcc-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f4dcc-129">reportPeriod</span></span>      | <span data-ttu-id="f4dcc-130">String</span><span class="sxs-lookup"><span data-stu-id="f4dcc-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f4dcc-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4dcc-131">JSON representation</span></span>

<span data-ttu-id="f4dcc-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4dcc-132">The following is a JSON representation of the resource.</span></span>

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
