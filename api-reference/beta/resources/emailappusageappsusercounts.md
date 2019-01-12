---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970379"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="cb12e-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb12e-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cb12e-104">属性</span><span class="sxs-lookup"><span data-stu-id="cb12e-104">Properties</span></span>

| <span data-ttu-id="cb12e-105">属性</span><span class="sxs-lookup"><span data-stu-id="cb12e-105">Property</span></span>          | <span data-ttu-id="cb12e-106">类型</span><span class="sxs-lookup"><span data-stu-id="cb12e-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="cb12e-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cb12e-107">reportRefreshDate</span></span> | <span data-ttu-id="cb12e-108">日期</span><span class="sxs-lookup"><span data-stu-id="cb12e-108">Date</span></span>   |
| <span data-ttu-id="cb12e-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="cb12e-109">mailForMac</span></span>        | <span data-ttu-id="cb12e-110">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-110">Int64</span></span>  |
| <span data-ttu-id="cb12e-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="cb12e-111">outlookForMac</span></span>     | <span data-ttu-id="cb12e-112">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-112">Int64</span></span>  |
| <span data-ttu-id="cb12e-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="cb12e-113">outlookForWindows</span></span> | <span data-ttu-id="cb12e-114">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-114">Int64</span></span>  |
| <span data-ttu-id="cb12e-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="cb12e-115">outlookForMobile</span></span>  | <span data-ttu-id="cb12e-116">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-116">Int64</span></span>  |
| <span data-ttu-id="cb12e-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="cb12e-117">otherForMobile</span></span>    | <span data-ttu-id="cb12e-118">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-118">Int64</span></span>  |
| <span data-ttu-id="cb12e-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="cb12e-119">outlookForWeb</span></span>     | <span data-ttu-id="cb12e-120">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-120">Int64</span></span>  |
| <span data-ttu-id="cb12e-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="cb12e-121">pop3App</span></span>           | <span data-ttu-id="cb12e-122">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-122">Int64</span></span>  |
| <span data-ttu-id="cb12e-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="cb12e-123">imap4App</span></span>          | <span data-ttu-id="cb12e-124">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-124">Int64</span></span>  |
| <span data-ttu-id="cb12e-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="cb12e-125">smtpApp</span></span>           | <span data-ttu-id="cb12e-126">Int64</span><span class="sxs-lookup"><span data-stu-id="cb12e-126">Int64</span></span>  |
| <span data-ttu-id="cb12e-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cb12e-127">reportPeriod</span></span>      | <span data-ttu-id="cb12e-128">String</span><span class="sxs-lookup"><span data-stu-id="cb12e-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cb12e-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb12e-129">JSON representation</span></span>

<span data-ttu-id="cb12e-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb12e-130">The following is a JSON representation of the resource.</span></span>

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
