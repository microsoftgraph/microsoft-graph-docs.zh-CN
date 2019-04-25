---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542830"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="125ca-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="125ca-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="125ca-104">属性</span><span class="sxs-lookup"><span data-stu-id="125ca-104">Properties</span></span>

| <span data-ttu-id="125ca-105">属性</span><span class="sxs-lookup"><span data-stu-id="125ca-105">Property</span></span>          | <span data-ttu-id="125ca-106">类型</span><span class="sxs-lookup"><span data-stu-id="125ca-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="125ca-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="125ca-107">reportRefreshDate</span></span> | <span data-ttu-id="125ca-108">Date</span><span class="sxs-lookup"><span data-stu-id="125ca-108">Date</span></span>              |
| <span data-ttu-id="125ca-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="125ca-109">userPrincipalName</span></span> | <span data-ttu-id="125ca-110">String</span><span class="sxs-lookup"><span data-stu-id="125ca-110">String</span></span>            |
| <span data-ttu-id="125ca-111">displayName</span><span class="sxs-lookup"><span data-stu-id="125ca-111">displayName</span></span>       | <span data-ttu-id="125ca-112">String</span><span class="sxs-lookup"><span data-stu-id="125ca-112">String</span></span>            |
| <span data-ttu-id="125ca-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="125ca-113">isDeleted</span></span>         | <span data-ttu-id="125ca-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="125ca-114">Boolean</span></span>           |
| <span data-ttu-id="125ca-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="125ca-115">deletedDate</span></span>       | <span data-ttu-id="125ca-116">Date</span><span class="sxs-lookup"><span data-stu-id="125ca-116">Date</span></span>              |
| <span data-ttu-id="125ca-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="125ca-117">lastActivityDate</span></span>  | <span data-ttu-id="125ca-118">Date</span><span class="sxs-lookup"><span data-stu-id="125ca-118">Date</span></span>              |
| <span data-ttu-id="125ca-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="125ca-119">sendCount</span></span>         | <span data-ttu-id="125ca-120">Int64</span><span class="sxs-lookup"><span data-stu-id="125ca-120">Int64</span></span>             |
| <span data-ttu-id="125ca-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="125ca-121">receiveCount</span></span>      | <span data-ttu-id="125ca-122">Int64</span><span class="sxs-lookup"><span data-stu-id="125ca-122">Int64</span></span>             |
| <span data-ttu-id="125ca-123">readCount</span><span class="sxs-lookup"><span data-stu-id="125ca-123">readCount</span></span>         | <span data-ttu-id="125ca-124">Int64</span><span class="sxs-lookup"><span data-stu-id="125ca-124">Int64</span></span>             |
| <span data-ttu-id="125ca-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="125ca-125">assignedProducts</span></span>  | <span data-ttu-id="125ca-126">String collection</span><span class="sxs-lookup"><span data-stu-id="125ca-126">String collection</span></span> |
| <span data-ttu-id="125ca-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="125ca-127">reportPeriod</span></span>      | <span data-ttu-id="125ca-128">String</span><span class="sxs-lookup"><span data-stu-id="125ca-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="125ca-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="125ca-129">JSON representation</span></span>

<span data-ttu-id="125ca-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="125ca-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "sendCount": 1024, 
  "receiveCount": 1024, 
  "readCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
