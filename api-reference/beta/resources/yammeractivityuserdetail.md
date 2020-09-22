---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: eb17035f0d062d55a3607dd30f31459b79b8400c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971368"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="3e1ea-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e1ea-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="3e1ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e1ea-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="3e1ea-105">属性</span><span class="sxs-lookup"><span data-stu-id="3e1ea-105">Properties</span></span>

| <span data-ttu-id="3e1ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="3e1ea-106">Property</span></span>          | <span data-ttu-id="3e1ea-107">类型</span><span class="sxs-lookup"><span data-stu-id="3e1ea-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="3e1ea-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="3e1ea-108">reportRefreshDate</span></span> | <span data-ttu-id="3e1ea-109">日期</span><span class="sxs-lookup"><span data-stu-id="3e1ea-109">Date</span></span>              |
| <span data-ttu-id="3e1ea-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3e1ea-110">userPrincipalName</span></span> | <span data-ttu-id="3e1ea-111">String</span><span class="sxs-lookup"><span data-stu-id="3e1ea-111">String</span></span>            |
| <span data-ttu-id="3e1ea-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3e1ea-112">displayName</span></span>       | <span data-ttu-id="3e1ea-113">String</span><span class="sxs-lookup"><span data-stu-id="3e1ea-113">String</span></span>            |
| <span data-ttu-id="3e1ea-114">userState</span><span class="sxs-lookup"><span data-stu-id="3e1ea-114">userState</span></span>         | <span data-ttu-id="3e1ea-115">String</span><span class="sxs-lookup"><span data-stu-id="3e1ea-115">String</span></span>            |
| <span data-ttu-id="3e1ea-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="3e1ea-116">stateChangeDate</span></span>   | <span data-ttu-id="3e1ea-117">日期</span><span class="sxs-lookup"><span data-stu-id="3e1ea-117">Date</span></span>              |
| <span data-ttu-id="3e1ea-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="3e1ea-118">lastActivityDate</span></span>  | <span data-ttu-id="3e1ea-119">日期</span><span class="sxs-lookup"><span data-stu-id="3e1ea-119">Date</span></span>              |
| <span data-ttu-id="3e1ea-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="3e1ea-120">postedCount</span></span>       | <span data-ttu-id="3e1ea-121">Int64</span><span class="sxs-lookup"><span data-stu-id="3e1ea-121">Int64</span></span>             |
| <span data-ttu-id="3e1ea-122">readCount</span><span class="sxs-lookup"><span data-stu-id="3e1ea-122">readCount</span></span>         | <span data-ttu-id="3e1ea-123">Int64</span><span class="sxs-lookup"><span data-stu-id="3e1ea-123">Int64</span></span>             |
| <span data-ttu-id="3e1ea-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="3e1ea-124">likedCount</span></span>        | <span data-ttu-id="3e1ea-125">Int64</span><span class="sxs-lookup"><span data-stu-id="3e1ea-125">Int64</span></span>             |
| <span data-ttu-id="3e1ea-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="3e1ea-126">assignedProducts</span></span>  | <span data-ttu-id="3e1ea-127">String collection</span><span class="sxs-lookup"><span data-stu-id="3e1ea-127">String collection</span></span> |
| <span data-ttu-id="3e1ea-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="3e1ea-128">reportPeriod</span></span>      | <span data-ttu-id="3e1ea-129">String</span><span class="sxs-lookup"><span data-stu-id="3e1ea-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="3e1ea-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e1ea-130">JSON representation</span></span>

<span data-ttu-id="3e1ea-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e1ea-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userState": "String", 
  "stateChangeDate": "Date", 
  "lastActivityDate": "Date", 
  "postedCount": 1024, 
  "readCount": 1024, 
  "likedCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```


