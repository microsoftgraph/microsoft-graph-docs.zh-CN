---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 76ec180ceb239f79c420f26b48521e9bc7e81787
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979481"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="58476-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="58476-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="58476-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58476-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="58476-105">属性</span><span class="sxs-lookup"><span data-stu-id="58476-105">Properties</span></span>

| <span data-ttu-id="58476-106">属性</span><span class="sxs-lookup"><span data-stu-id="58476-106">Property</span></span>          | <span data-ttu-id="58476-107">类型</span><span class="sxs-lookup"><span data-stu-id="58476-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="58476-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="58476-108">reportRefreshDate</span></span> | <span data-ttu-id="58476-109">日期</span><span class="sxs-lookup"><span data-stu-id="58476-109">Date</span></span>              |
| <span data-ttu-id="58476-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58476-110">userPrincipalName</span></span> | <span data-ttu-id="58476-111">String</span><span class="sxs-lookup"><span data-stu-id="58476-111">String</span></span>            |
| <span data-ttu-id="58476-112">displayName</span><span class="sxs-lookup"><span data-stu-id="58476-112">displayName</span></span>       | <span data-ttu-id="58476-113">String</span><span class="sxs-lookup"><span data-stu-id="58476-113">String</span></span>            |
| <span data-ttu-id="58476-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="58476-114">isDeleted</span></span>         | <span data-ttu-id="58476-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="58476-115">Boolean</span></span>           |
| <span data-ttu-id="58476-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="58476-116">deletedDate</span></span>       | <span data-ttu-id="58476-117">日期</span><span class="sxs-lookup"><span data-stu-id="58476-117">Date</span></span>              |
| <span data-ttu-id="58476-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="58476-118">lastActivityDate</span></span>  | <span data-ttu-id="58476-119">日期</span><span class="sxs-lookup"><span data-stu-id="58476-119">Date</span></span>              |
| <span data-ttu-id="58476-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="58476-120">sendCount</span></span>         | <span data-ttu-id="58476-121">Int64</span><span class="sxs-lookup"><span data-stu-id="58476-121">Int64</span></span>             |
| <span data-ttu-id="58476-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="58476-122">receiveCount</span></span>      | <span data-ttu-id="58476-123">Int64</span><span class="sxs-lookup"><span data-stu-id="58476-123">Int64</span></span>             |
| <span data-ttu-id="58476-124">readCount</span><span class="sxs-lookup"><span data-stu-id="58476-124">readCount</span></span>         | <span data-ttu-id="58476-125">Int64</span><span class="sxs-lookup"><span data-stu-id="58476-125">Int64</span></span>             |
| <span data-ttu-id="58476-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="58476-126">assignedProducts</span></span>  | <span data-ttu-id="58476-127">String collection</span><span class="sxs-lookup"><span data-stu-id="58476-127">String collection</span></span> |
| <span data-ttu-id="58476-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="58476-128">reportPeriod</span></span>      | <span data-ttu-id="58476-129">String</span><span class="sxs-lookup"><span data-stu-id="58476-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="58476-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58476-130">JSON representation</span></span>

<span data-ttu-id="58476-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58476-131">The following is a JSON representation of the resource.</span></span>

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


