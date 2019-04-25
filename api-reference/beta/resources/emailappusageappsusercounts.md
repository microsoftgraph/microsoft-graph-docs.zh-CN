---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 220770fab755c0e345af23f3fc3113732af63ff0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542809"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="1b040-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b040-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1b040-104">属性</span><span class="sxs-lookup"><span data-stu-id="1b040-104">Properties</span></span>

| <span data-ttu-id="1b040-105">属性</span><span class="sxs-lookup"><span data-stu-id="1b040-105">Property</span></span>          | <span data-ttu-id="1b040-106">类型</span><span class="sxs-lookup"><span data-stu-id="1b040-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="1b040-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1b040-107">reportRefreshDate</span></span> | <span data-ttu-id="1b040-108">Date</span><span class="sxs-lookup"><span data-stu-id="1b040-108">Date</span></span>   |
| <span data-ttu-id="1b040-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="1b040-109">mailForMac</span></span>        | <span data-ttu-id="1b040-110">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-110">Int64</span></span>  |
| <span data-ttu-id="1b040-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="1b040-111">outlookForMac</span></span>     | <span data-ttu-id="1b040-112">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-112">Int64</span></span>  |
| <span data-ttu-id="1b040-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="1b040-113">outlookForWindows</span></span> | <span data-ttu-id="1b040-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-114">Int64</span></span>  |
| <span data-ttu-id="1b040-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="1b040-115">outlookForMobile</span></span>  | <span data-ttu-id="1b040-116">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-116">Int64</span></span>  |
| <span data-ttu-id="1b040-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="1b040-117">otherForMobile</span></span>    | <span data-ttu-id="1b040-118">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-118">Int64</span></span>  |
| <span data-ttu-id="1b040-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="1b040-119">outlookForWeb</span></span>     | <span data-ttu-id="1b040-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-120">Int64</span></span>  |
| <span data-ttu-id="1b040-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="1b040-121">pop3App</span></span>           | <span data-ttu-id="1b040-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-122">Int64</span></span>  |
| <span data-ttu-id="1b040-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="1b040-123">imap4App</span></span>          | <span data-ttu-id="1b040-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-124">Int64</span></span>  |
| <span data-ttu-id="1b040-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="1b040-125">smtpApp</span></span>           | <span data-ttu-id="1b040-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1b040-126">Int64</span></span>  |
| <span data-ttu-id="1b040-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1b040-127">reportPeriod</span></span>      | <span data-ttu-id="1b040-128">String</span><span class="sxs-lookup"><span data-stu-id="1b040-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1b040-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b040-129">JSON representation</span></span>

<span data-ttu-id="1b040-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b040-130">The following is a JSON representation of the resource.</span></span>

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
