---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: a018776f092e9b7f378e8069666d015e1cd3e4a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835446"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="460c0-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="460c0-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="460c0-104">属性</span><span class="sxs-lookup"><span data-stu-id="460c0-104">Properties</span></span>

| <span data-ttu-id="460c0-105">属性</span><span class="sxs-lookup"><span data-stu-id="460c0-105">Property</span></span>          | <span data-ttu-id="460c0-106">类型</span><span class="sxs-lookup"><span data-stu-id="460c0-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="460c0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="460c0-107">reportRefreshDate</span></span> | <span data-ttu-id="460c0-108">日期</span><span class="sxs-lookup"><span data-stu-id="460c0-108">Date</span></span>   |
| <span data-ttu-id="460c0-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="460c0-109">mailForMac</span></span>        | <span data-ttu-id="460c0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-110">Int64</span></span>  |
| <span data-ttu-id="460c0-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="460c0-111">outlookForMac</span></span>     | <span data-ttu-id="460c0-112">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-112">Int64</span></span>  |
| <span data-ttu-id="460c0-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="460c0-113">outlookForWindows</span></span> | <span data-ttu-id="460c0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-114">Int64</span></span>  |
| <span data-ttu-id="460c0-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="460c0-115">outlookForMobile</span></span>  | <span data-ttu-id="460c0-116">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-116">Int64</span></span>  |
| <span data-ttu-id="460c0-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="460c0-117">otherForMobile</span></span>    | <span data-ttu-id="460c0-118">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-118">Int64</span></span>  |
| <span data-ttu-id="460c0-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="460c0-119">outlookForWeb</span></span>     | <span data-ttu-id="460c0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-120">Int64</span></span>  |
| <span data-ttu-id="460c0-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="460c0-121">pop3App</span></span>           | <span data-ttu-id="460c0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-122">Int64</span></span>  |
| <span data-ttu-id="460c0-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="460c0-123">imap4App</span></span>          | <span data-ttu-id="460c0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-124">Int64</span></span>  |
| <span data-ttu-id="460c0-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="460c0-125">smtpApp</span></span>           | <span data-ttu-id="460c0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="460c0-126">Int64</span></span>  |
| <span data-ttu-id="460c0-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="460c0-127">reportDate</span></span>        | <span data-ttu-id="460c0-128">日期</span><span class="sxs-lookup"><span data-stu-id="460c0-128">Date</span></span>   |
| <span data-ttu-id="460c0-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="460c0-129">reportPeriod</span></span>      | <span data-ttu-id="460c0-130">String</span><span class="sxs-lookup"><span data-stu-id="460c0-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="460c0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="460c0-131">JSON representation</span></span>

<span data-ttu-id="460c0-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="460c0-132">The following is a JSON representation of the resource.</span></span>

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
