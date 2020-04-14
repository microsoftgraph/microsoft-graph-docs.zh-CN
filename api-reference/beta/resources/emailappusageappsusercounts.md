---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: fb06e9dfe56edb0e7882d0cdce8ee4564375ed93
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440560"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="f13b2-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f13b2-103">emailAppUsageAppsUserCounts resource type</span></span>

<span data-ttu-id="f13b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f13b2-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="f13b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="f13b2-105">Properties</span></span>

| <span data-ttu-id="f13b2-106">属性</span><span class="sxs-lookup"><span data-stu-id="f13b2-106">Property</span></span>          | <span data-ttu-id="f13b2-107">类型</span><span class="sxs-lookup"><span data-stu-id="f13b2-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="f13b2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f13b2-108">reportRefreshDate</span></span> | <span data-ttu-id="f13b2-109">日期</span><span class="sxs-lookup"><span data-stu-id="f13b2-109">Date</span></span>   |
| <span data-ttu-id="f13b2-110">mailForMac</span><span class="sxs-lookup"><span data-stu-id="f13b2-110">mailForMac</span></span>        | <span data-ttu-id="f13b2-111">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-111">Int64</span></span>  |
| <span data-ttu-id="f13b2-112">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="f13b2-112">outlookForMac</span></span>     | <span data-ttu-id="f13b2-113">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-113">Int64</span></span>  |
| <span data-ttu-id="f13b2-114">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="f13b2-114">outlookForWindows</span></span> | <span data-ttu-id="f13b2-115">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-115">Int64</span></span>  |
| <span data-ttu-id="f13b2-116">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="f13b2-116">outlookForMobile</span></span>  | <span data-ttu-id="f13b2-117">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-117">Int64</span></span>  |
| <span data-ttu-id="f13b2-118">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="f13b2-118">otherForMobile</span></span>    | <span data-ttu-id="f13b2-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-119">Int64</span></span>  |
| <span data-ttu-id="f13b2-120">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="f13b2-120">outlookForWeb</span></span>     | <span data-ttu-id="f13b2-121">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-121">Int64</span></span>  |
| <span data-ttu-id="f13b2-122">pop3App</span><span class="sxs-lookup"><span data-stu-id="f13b2-122">pop3App</span></span>           | <span data-ttu-id="f13b2-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-123">Int64</span></span>  |
| <span data-ttu-id="f13b2-124">imap4App</span><span class="sxs-lookup"><span data-stu-id="f13b2-124">imap4App</span></span>          | <span data-ttu-id="f13b2-125">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-125">Int64</span></span>  |
| <span data-ttu-id="f13b2-126">smtpApp</span><span class="sxs-lookup"><span data-stu-id="f13b2-126">smtpApp</span></span>           | <span data-ttu-id="f13b2-127">Int64</span><span class="sxs-lookup"><span data-stu-id="f13b2-127">Int64</span></span>  |
| <span data-ttu-id="f13b2-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f13b2-128">reportPeriod</span></span>      | <span data-ttu-id="f13b2-129">String</span><span class="sxs-lookup"><span data-stu-id="f13b2-129">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f13b2-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f13b2-130">JSON representation</span></span>

<span data-ttu-id="f13b2-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f13b2-131">The following is a JSON representation of the resource.</span></span>

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
