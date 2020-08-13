---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 922ebf14f59d60a988fe77ee36ce04d9c76befec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519027"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="c4105-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4105-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="c4105-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4105-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c4105-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4105-105">Properties</span></span>

| <span data-ttu-id="c4105-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4105-106">Property</span></span>          | <span data-ttu-id="c4105-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4105-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="c4105-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c4105-108">reportRefreshDate</span></span> | <span data-ttu-id="c4105-109">日期</span><span class="sxs-lookup"><span data-stu-id="c4105-109">Date</span></span>              |
| <span data-ttu-id="c4105-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c4105-110">userPrincipalName</span></span> | <span data-ttu-id="c4105-111">String</span><span class="sxs-lookup"><span data-stu-id="c4105-111">String</span></span>            |
| <span data-ttu-id="c4105-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c4105-112">displayName</span></span>       | <span data-ttu-id="c4105-113">String</span><span class="sxs-lookup"><span data-stu-id="c4105-113">String</span></span>            |
| <span data-ttu-id="c4105-114">userState</span><span class="sxs-lookup"><span data-stu-id="c4105-114">userState</span></span>         | <span data-ttu-id="c4105-115">String</span><span class="sxs-lookup"><span data-stu-id="c4105-115">String</span></span>            |
| <span data-ttu-id="c4105-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="c4105-116">stateChangeDate</span></span>   | <span data-ttu-id="c4105-117">日期</span><span class="sxs-lookup"><span data-stu-id="c4105-117">Date</span></span>              |
| <span data-ttu-id="c4105-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c4105-118">lastActivityDate</span></span>  | <span data-ttu-id="c4105-119">日期</span><span class="sxs-lookup"><span data-stu-id="c4105-119">Date</span></span>              |
| <span data-ttu-id="c4105-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="c4105-120">postedCount</span></span>       | <span data-ttu-id="c4105-121">Int64</span><span class="sxs-lookup"><span data-stu-id="c4105-121">Int64</span></span>             |
| <span data-ttu-id="c4105-122">readCount</span><span class="sxs-lookup"><span data-stu-id="c4105-122">readCount</span></span>         | <span data-ttu-id="c4105-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c4105-123">Int64</span></span>             |
| <span data-ttu-id="c4105-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="c4105-124">likedCount</span></span>        | <span data-ttu-id="c4105-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c4105-125">Int64</span></span>             |
| <span data-ttu-id="c4105-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c4105-126">assignedProducts</span></span>  | <span data-ttu-id="c4105-127">String collection</span><span class="sxs-lookup"><span data-stu-id="c4105-127">String collection</span></span> |
| <span data-ttu-id="c4105-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c4105-128">reportPeriod</span></span>      | <span data-ttu-id="c4105-129">String</span><span class="sxs-lookup"><span data-stu-id="c4105-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c4105-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4105-130">JSON representation</span></span>

<span data-ttu-id="c4105-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4105-131">The following is a JSON representation of the resource.</span></span>

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
