---
title: emailAppUsageUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d8af9e9337c68fcd4434514b85fa9217c79add26
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972171"
---
# <a name="emailappusageusercounts-resource-type"></a><span data-ttu-id="faf1f-103">emailAppUsageUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="faf1f-103">emailAppUsageUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="faf1f-104">属性</span><span class="sxs-lookup"><span data-stu-id="faf1f-104">Properties</span></span>

| <span data-ttu-id="faf1f-105">属性</span><span class="sxs-lookup"><span data-stu-id="faf1f-105">Property</span></span>          | <span data-ttu-id="faf1f-106">类型</span><span class="sxs-lookup"><span data-stu-id="faf1f-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="faf1f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="faf1f-107">reportRefreshDate</span></span> | <span data-ttu-id="faf1f-108">日期</span><span class="sxs-lookup"><span data-stu-id="faf1f-108">Date</span></span>   |
| <span data-ttu-id="faf1f-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="faf1f-109">mailForMac</span></span>        | <span data-ttu-id="faf1f-110">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-110">Int64</span></span>  |
| <span data-ttu-id="faf1f-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="faf1f-111">outlookForMac</span></span>     | <span data-ttu-id="faf1f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-112">Int64</span></span>  |
| <span data-ttu-id="faf1f-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="faf1f-113">outlookForWindows</span></span> | <span data-ttu-id="faf1f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-114">Int64</span></span>  |
| <span data-ttu-id="faf1f-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="faf1f-115">outlookForMobile</span></span>  | <span data-ttu-id="faf1f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-116">Int64</span></span>  |
| <span data-ttu-id="faf1f-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="faf1f-117">otherForMobile</span></span>    | <span data-ttu-id="faf1f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-118">Int64</span></span>  |
| <span data-ttu-id="faf1f-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="faf1f-119">outlookForWeb</span></span>     | <span data-ttu-id="faf1f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-120">Int64</span></span>  |
| <span data-ttu-id="faf1f-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="faf1f-121">pop3App</span></span>           | <span data-ttu-id="faf1f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-122">Int64</span></span>  |
| <span data-ttu-id="faf1f-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="faf1f-123">imap4App</span></span>          | <span data-ttu-id="faf1f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-124">Int64</span></span>  |
| <span data-ttu-id="faf1f-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="faf1f-125">smtpApp</span></span>           | <span data-ttu-id="faf1f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="faf1f-126">Int64</span></span>  |
| <span data-ttu-id="faf1f-127">reportDate</span><span class="sxs-lookup"><span data-stu-id="faf1f-127">reportDate</span></span>        | <span data-ttu-id="faf1f-128">日期</span><span class="sxs-lookup"><span data-stu-id="faf1f-128">Date</span></span>   |
| <span data-ttu-id="faf1f-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="faf1f-129">reportPeriod</span></span>      | <span data-ttu-id="faf1f-130">String</span><span class="sxs-lookup"><span data-stu-id="faf1f-130">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="faf1f-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faf1f-131">JSON representation</span></span>

<span data-ttu-id="faf1f-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faf1f-132">The following is a JSON representation of the resource.</span></span>

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
