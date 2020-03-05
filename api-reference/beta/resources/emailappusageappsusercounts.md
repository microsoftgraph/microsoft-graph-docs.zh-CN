---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d34ceaf4450a66f07c0678e55db344adc20bb0b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499496"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="89c2e-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="89c2e-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="89c2e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="89c2e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="89c2e-105">属性</span><span class="sxs-lookup"><span data-stu-id="89c2e-105">Properties</span></span>

| <span data-ttu-id="89c2e-106">属性</span><span class="sxs-lookup"><span data-stu-id="89c2e-106">Property</span></span>          | <span data-ttu-id="89c2e-107">类型</span><span class="sxs-lookup"><span data-stu-id="89c2e-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="89c2e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="89c2e-108">reportRefreshDate</span></span> | <span data-ttu-id="89c2e-109">日期</span><span class="sxs-lookup"><span data-stu-id="89c2e-109">Date</span></span>   |
| <span data-ttu-id="89c2e-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="89c2e-110">mailForMac</span></span>        | <span data-ttu-id="89c2e-111">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-111">Int64</span></span>  |
| <span data-ttu-id="89c2e-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="89c2e-112">outlookForMac</span></span>     | <span data-ttu-id="89c2e-113">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-113">Int64</span></span>  |
| <span data-ttu-id="89c2e-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="89c2e-114">outlookForWindows</span></span> | <span data-ttu-id="89c2e-115">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-115">Int64</span></span>  |
| <span data-ttu-id="89c2e-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="89c2e-116">outlookForMobile</span></span>  | <span data-ttu-id="89c2e-117">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-117">Int64</span></span>  |
| <span data-ttu-id="89c2e-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="89c2e-118">otherForMobile</span></span>    | <span data-ttu-id="89c2e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-119">Int64</span></span>  |
| <span data-ttu-id="89c2e-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="89c2e-120">outlookForWeb</span></span>     | <span data-ttu-id="89c2e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-121">Int64</span></span>  |
| <span data-ttu-id="89c2e-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="89c2e-122">pop3App</span></span>           | <span data-ttu-id="89c2e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-123">Int64</span></span>  |
| <span data-ttu-id="89c2e-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="89c2e-124">imap4App</span></span>          | <span data-ttu-id="89c2e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-125">Int64</span></span>  |
| <span data-ttu-id="89c2e-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="89c2e-126">smtpApp</span></span>           | <span data-ttu-id="89c2e-127">Int64</span><span class="sxs-lookup"><span data-stu-id="89c2e-127">Int64</span></span>  |
| <span data-ttu-id="89c2e-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="89c2e-128">reportPeriod</span></span>      | <span data-ttu-id="89c2e-129">String</span><span class="sxs-lookup"><span data-stu-id="89c2e-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="89c2e-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89c2e-130">JSON representation</span></span>

<span data-ttu-id="89c2e-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89c2e-131">The following is a JSON representation of the resource.</span></span>

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
