---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0ca694c5d416dcc062984ba03a3521a39a010a87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972178"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="5c873-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c873-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5c873-104">属性</span><span class="sxs-lookup"><span data-stu-id="5c873-104">Properties</span></span>

| <span data-ttu-id="5c873-105">属性</span><span class="sxs-lookup"><span data-stu-id="5c873-105">Property</span></span>          | <span data-ttu-id="5c873-106">类型</span><span class="sxs-lookup"><span data-stu-id="5c873-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="5c873-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5c873-107">reportRefreshDate</span></span> | <span data-ttu-id="5c873-108">日期</span><span class="sxs-lookup"><span data-stu-id="5c873-108">Date</span></span>   |
| <span data-ttu-id="5c873-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="5c873-109">mailForMac</span></span>        | <span data-ttu-id="5c873-110">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-110">Int64</span></span>  |
| <span data-ttu-id="5c873-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="5c873-111">outlookForMac</span></span>     | <span data-ttu-id="5c873-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-112">Int64</span></span>  |
| <span data-ttu-id="5c873-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="5c873-113">outlookForWindows</span></span> | <span data-ttu-id="5c873-114">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-114">Int64</span></span>  |
| <span data-ttu-id="5c873-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="5c873-115">outlookForMobile</span></span>  | <span data-ttu-id="5c873-116">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-116">Int64</span></span>  |
| <span data-ttu-id="5c873-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="5c873-117">otherForMobile</span></span>    | <span data-ttu-id="5c873-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-118">Int64</span></span>  |
| <span data-ttu-id="5c873-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="5c873-119">outlookForWeb</span></span>     | <span data-ttu-id="5c873-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-120">Int64</span></span>  |
| <span data-ttu-id="5c873-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="5c873-121">pop3App</span></span>           | <span data-ttu-id="5c873-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-122">Int64</span></span>  |
| <span data-ttu-id="5c873-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="5c873-123">imap4App</span></span>          | <span data-ttu-id="5c873-124">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-124">Int64</span></span>  |
| <span data-ttu-id="5c873-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="5c873-125">smtpApp</span></span>           | <span data-ttu-id="5c873-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5c873-126">Int64</span></span>  |
| <span data-ttu-id="5c873-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5c873-127">reportPeriod</span></span>      | <span data-ttu-id="5c873-128">String</span><span class="sxs-lookup"><span data-stu-id="5c873-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5c873-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c873-129">JSON representation</span></span>

<span data-ttu-id="5c873-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c873-130">The following is a JSON representation of the resource.</span></span>

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
