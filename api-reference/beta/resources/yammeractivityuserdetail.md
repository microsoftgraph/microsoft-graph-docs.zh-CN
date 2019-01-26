---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: eea520e6024bb050001461fb5ada5c90ea2b2125
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575826"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="4e8df-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e8df-103">yammerActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4e8df-104">属性</span><span class="sxs-lookup"><span data-stu-id="4e8df-104">Properties</span></span>

| <span data-ttu-id="4e8df-105">属性</span><span class="sxs-lookup"><span data-stu-id="4e8df-105">Property</span></span>          | <span data-ttu-id="4e8df-106">类型</span><span class="sxs-lookup"><span data-stu-id="4e8df-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="4e8df-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4e8df-107">reportRefreshDate</span></span> | <span data-ttu-id="4e8df-108">Date</span><span class="sxs-lookup"><span data-stu-id="4e8df-108">Date</span></span>              |
| <span data-ttu-id="4e8df-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e8df-109">userPrincipalName</span></span> | <span data-ttu-id="4e8df-110">String</span><span class="sxs-lookup"><span data-stu-id="4e8df-110">String</span></span>            |
| <span data-ttu-id="4e8df-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4e8df-111">displayName</span></span>       | <span data-ttu-id="4e8df-112">String</span><span class="sxs-lookup"><span data-stu-id="4e8df-112">String</span></span>            |
| <span data-ttu-id="4e8df-113">userState</span><span class="sxs-lookup"><span data-stu-id="4e8df-113">userState</span></span>         | <span data-ttu-id="4e8df-114">String</span><span class="sxs-lookup"><span data-stu-id="4e8df-114">String</span></span>            |
| <span data-ttu-id="4e8df-115">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="4e8df-115">stateChangeDate</span></span>   | <span data-ttu-id="4e8df-116">Date</span><span class="sxs-lookup"><span data-stu-id="4e8df-116">Date</span></span>              |
| <span data-ttu-id="4e8df-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4e8df-117">lastActivityDate</span></span>  | <span data-ttu-id="4e8df-118">Date</span><span class="sxs-lookup"><span data-stu-id="4e8df-118">Date</span></span>              |
| <span data-ttu-id="4e8df-119">postedCount</span><span class="sxs-lookup"><span data-stu-id="4e8df-119">postedCount</span></span>       | <span data-ttu-id="4e8df-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4e8df-120">Int64</span></span>             |
| <span data-ttu-id="4e8df-121">readCount</span><span class="sxs-lookup"><span data-stu-id="4e8df-121">readCount</span></span>         | <span data-ttu-id="4e8df-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4e8df-122">Int64</span></span>             |
| <span data-ttu-id="4e8df-123">likedCount</span><span class="sxs-lookup"><span data-stu-id="4e8df-123">likedCount</span></span>        | <span data-ttu-id="4e8df-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4e8df-124">Int64</span></span>             |
| <span data-ttu-id="4e8df-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="4e8df-125">assignedProducts</span></span>  | <span data-ttu-id="4e8df-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="4e8df-126">String collection</span></span> |
| <span data-ttu-id="4e8df-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4e8df-127">reportPeriod</span></span>      | <span data-ttu-id="4e8df-128">String</span><span class="sxs-lookup"><span data-stu-id="4e8df-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4e8df-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e8df-129">JSON representation</span></span>

<span data-ttu-id="4e8df-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e8df-130">The following is a JSON representation of the resource.</span></span>

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
