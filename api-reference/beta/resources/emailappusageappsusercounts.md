---
title: emailAppUsageAppsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: e588a671129c6aa131bce781e3a6db0d44128f6d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044340"
---
# <a name="emailappusageappsusercounts-resource-type"></a><span data-ttu-id="b6daa-103">emailAppUsageAppsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6daa-103">emailAppUsageAppsUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="b6daa-104">属性</span><span class="sxs-lookup"><span data-stu-id="b6daa-104">Properties</span></span>

| <span data-ttu-id="b6daa-105">属性</span><span class="sxs-lookup"><span data-stu-id="b6daa-105">Property</span></span>          | <span data-ttu-id="b6daa-106">类型</span><span class="sxs-lookup"><span data-stu-id="b6daa-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b6daa-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b6daa-107">reportRefreshDate</span></span> | <span data-ttu-id="b6daa-108">日期</span><span class="sxs-lookup"><span data-stu-id="b6daa-108">Date</span></span>   |
| <span data-ttu-id="b6daa-109">mailForMac</span><span class="sxs-lookup"><span data-stu-id="b6daa-109">mailForMac</span></span>        | <span data-ttu-id="b6daa-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-110">Int64</span></span>  |
| <span data-ttu-id="b6daa-111">outlookForMac</span><span class="sxs-lookup"><span data-stu-id="b6daa-111">outlookForMac</span></span>     | <span data-ttu-id="b6daa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-112">Int64</span></span>  |
| <span data-ttu-id="b6daa-113">outlookForWindows</span><span class="sxs-lookup"><span data-stu-id="b6daa-113">outlookForWindows</span></span> | <span data-ttu-id="b6daa-114">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-114">Int64</span></span>  |
| <span data-ttu-id="b6daa-115">outlookForMobile</span><span class="sxs-lookup"><span data-stu-id="b6daa-115">outlookForMobile</span></span>  | <span data-ttu-id="b6daa-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-116">Int64</span></span>  |
| <span data-ttu-id="b6daa-117">otherForMobile</span><span class="sxs-lookup"><span data-stu-id="b6daa-117">otherForMobile</span></span>    | <span data-ttu-id="b6daa-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-118">Int64</span></span>  |
| <span data-ttu-id="b6daa-119">outlookForWeb</span><span class="sxs-lookup"><span data-stu-id="b6daa-119">outlookForWeb</span></span>     | <span data-ttu-id="b6daa-120">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-120">Int64</span></span>  |
| <span data-ttu-id="b6daa-121">pop3App</span><span class="sxs-lookup"><span data-stu-id="b6daa-121">pop3App</span></span>           | <span data-ttu-id="b6daa-122">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-122">Int64</span></span>  |
| <span data-ttu-id="b6daa-123">imap4App</span><span class="sxs-lookup"><span data-stu-id="b6daa-123">imap4App</span></span>          | <span data-ttu-id="b6daa-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-124">Int64</span></span>  |
| <span data-ttu-id="b6daa-125">smtpApp</span><span class="sxs-lookup"><span data-stu-id="b6daa-125">smtpApp</span></span>           | <span data-ttu-id="b6daa-126">Int64</span><span class="sxs-lookup"><span data-stu-id="b6daa-126">Int64</span></span>  |
| <span data-ttu-id="b6daa-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b6daa-127">reportPeriod</span></span>      | <span data-ttu-id="b6daa-128">String</span><span class="sxs-lookup"><span data-stu-id="b6daa-128">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b6daa-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6daa-129">JSON representation</span></span>

<span data-ttu-id="b6daa-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6daa-130">The following is a JSON representation of the resource.</span></span>

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
