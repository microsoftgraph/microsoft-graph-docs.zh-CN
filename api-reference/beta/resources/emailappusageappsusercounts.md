---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: efbc4ce75293237813e9a835cb45ff0bf0ec4b26
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807817"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="24061-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="24061-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="24061-104">属性</span><span class="sxs-lookup"><span data-stu-id="24061-104">Properties</span></span>

| <span data-ttu-id="24061-105">属性</span><span class="sxs-lookup"><span data-stu-id="24061-105">Property</span></span>          | <span data-ttu-id="24061-106">类型</span><span class="sxs-lookup"><span data-stu-id="24061-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="24061-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="24061-107">reportRefreshDate</span></span> | <span data-ttu-id="24061-108">日期</span><span class="sxs-lookup"><span data-stu-id="24061-108">Date</span></span>   |
| <span data-ttu-id="24061-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="24061-109">mailForMac</span></span>        | <span data-ttu-id="24061-110">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-110">Int64</span></span>  |
| <span data-ttu-id="24061-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="24061-111">outlookForMac</span></span>     | <span data-ttu-id="24061-112">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-112">Int64</span></span>  |
| <span data-ttu-id="24061-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="24061-113">outlookForWindows</span></span> | <span data-ttu-id="24061-114">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-114">Int64</span></span>  |
| <span data-ttu-id="24061-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="24061-115">outlookForMobile</span></span>  | <span data-ttu-id="24061-116">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-116">Int64</span></span>  |
| <span data-ttu-id="24061-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="24061-117">otherForMobile</span></span>    | <span data-ttu-id="24061-118">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-118">Int64</span></span>  |
| <span data-ttu-id="24061-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="24061-119">outlookForWeb</span></span>     | <span data-ttu-id="24061-120">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-120">Int64</span></span>  |
| <span data-ttu-id="24061-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="24061-121">pop3App</span></span>           | <span data-ttu-id="24061-122">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-122">Int64</span></span>  |
| <span data-ttu-id="24061-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="24061-123">imap4App</span></span>          | <span data-ttu-id="24061-124">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-124">Int64</span></span>  |
| <span data-ttu-id="24061-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="24061-125">smtpApp</span></span>           | <span data-ttu-id="24061-126">Int64</span><span class="sxs-lookup"><span data-stu-id="24061-126">Int64</span></span>  |
| <span data-ttu-id="24061-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="24061-127">reportPeriod</span></span>      | <span data-ttu-id="24061-128">String</span><span class="sxs-lookup"><span data-stu-id="24061-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24061-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24061-129">JSON representation</span></span>

<span data-ttu-id="24061-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24061-130">The following is a JSON representation of the resource.</span></span>

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
