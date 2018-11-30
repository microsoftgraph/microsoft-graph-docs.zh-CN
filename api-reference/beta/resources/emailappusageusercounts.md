---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: c8669c8a34987bc1e71152ae717f9be3ba101107
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046879"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="9faa5-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="9faa5-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9faa5-104">属性</span><span class="sxs-lookup"><span data-stu-id="9faa5-104">Properties</span></span>

| <span data-ttu-id="9faa5-105">属性</span><span class="sxs-lookup"><span data-stu-id="9faa5-105">Property</span></span>          | <span data-ttu-id="9faa5-106">类型</span><span class="sxs-lookup"><span data-stu-id="9faa5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="9faa5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9faa5-107">reportRefreshDate</span></span> | <span data-ttu-id="9faa5-108">日期</span><span class="sxs-lookup"><span data-stu-id="9faa5-108">Date</span></span>   |
| <span data-ttu-id="9faa5-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="9faa5-109">mailForMac</span></span>        | <span data-ttu-id="9faa5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-110">Int64</span></span>  |
| <span data-ttu-id="9faa5-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="9faa5-111">outlookForMac</span></span>     | <span data-ttu-id="9faa5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-112">Int64</span></span>  |
| <span data-ttu-id="9faa5-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="9faa5-113">outlookForWindows</span></span> | <span data-ttu-id="9faa5-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-114">Int64</span></span>  |
| <span data-ttu-id="9faa5-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="9faa5-115">outlookForMobile</span></span>  | <span data-ttu-id="9faa5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-116">Int64</span></span>  |
| <span data-ttu-id="9faa5-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="9faa5-117">otherForMobile</span></span>    | <span data-ttu-id="9faa5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-118">Int64</span></span>  |
| <span data-ttu-id="9faa5-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="9faa5-119">outlookForWeb</span></span>     | <span data-ttu-id="9faa5-120">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-120">Int64</span></span>  |
| <span data-ttu-id="9faa5-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="9faa5-121">pop3App</span></span>           | <span data-ttu-id="9faa5-122">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-122">Int64</span></span>  |
| <span data-ttu-id="9faa5-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="9faa5-123">imap4App</span></span>          | <span data-ttu-id="9faa5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-124">Int64</span></span>  |
| <span data-ttu-id="9faa5-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="9faa5-125">smtpApp</span></span>           | <span data-ttu-id="9faa5-126">Int64</span><span class="sxs-lookup"><span data-stu-id="9faa5-126">Int64</span></span>  |
| <span data-ttu-id="9faa5-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="9faa5-127">reportDate</span></span>        | <span data-ttu-id="9faa5-128">日期</span><span class="sxs-lookup"><span data-stu-id="9faa5-128">Date</span></span>   |
| <span data-ttu-id="9faa5-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9faa5-129">reportPeriod</span></span>      | <span data-ttu-id="9faa5-130">String</span><span class="sxs-lookup"><span data-stu-id="9faa5-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9faa5-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9faa5-131">JSON representation</span></span>

<span data-ttu-id="9faa5-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9faa5-132">The following is a JSON representation of the resource.</span></span>

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
