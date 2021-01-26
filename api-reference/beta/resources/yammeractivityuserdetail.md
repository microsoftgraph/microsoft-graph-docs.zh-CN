---
title: yammerActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 749076f407b49ff4fd408a095312ac49ea008bc1
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982395"
---
# <a name="yammeractivityuserdetail-resource-type"></a><span data-ttu-id="d09db-103">yammerActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d09db-103">yammerActivityUserDetail resource type</span></span>

<span data-ttu-id="d09db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d09db-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d09db-105">属性</span><span class="sxs-lookup"><span data-stu-id="d09db-105">Properties</span></span>

| <span data-ttu-id="d09db-106">属性</span><span class="sxs-lookup"><span data-stu-id="d09db-106">Property</span></span>          | <span data-ttu-id="d09db-107">类型</span><span class="sxs-lookup"><span data-stu-id="d09db-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="d09db-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d09db-108">reportRefreshDate</span></span> | <span data-ttu-id="d09db-109">日期</span><span class="sxs-lookup"><span data-stu-id="d09db-109">Date</span></span>              |
| <span data-ttu-id="d09db-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d09db-110">userPrincipalName</span></span> | <span data-ttu-id="d09db-111">String</span><span class="sxs-lookup"><span data-stu-id="d09db-111">String</span></span>            |
| <span data-ttu-id="d09db-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d09db-112">displayName</span></span>       | <span data-ttu-id="d09db-113">String</span><span class="sxs-lookup"><span data-stu-id="d09db-113">String</span></span>            |
| <span data-ttu-id="d09db-114">userState</span><span class="sxs-lookup"><span data-stu-id="d09db-114">userState</span></span>         | <span data-ttu-id="d09db-115">String</span><span class="sxs-lookup"><span data-stu-id="d09db-115">String</span></span>            |
| <span data-ttu-id="d09db-116">stateChangeDate</span><span class="sxs-lookup"><span data-stu-id="d09db-116">stateChangeDate</span></span>   | <span data-ttu-id="d09db-117">日期</span><span class="sxs-lookup"><span data-stu-id="d09db-117">Date</span></span>              |
| <span data-ttu-id="d09db-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d09db-118">lastActivityDate</span></span>  | <span data-ttu-id="d09db-119">日期</span><span class="sxs-lookup"><span data-stu-id="d09db-119">Date</span></span>              |
| <span data-ttu-id="d09db-120">postedCount</span><span class="sxs-lookup"><span data-stu-id="d09db-120">postedCount</span></span>       | <span data-ttu-id="d09db-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d09db-121">Int64</span></span>             |
| <span data-ttu-id="d09db-122">readCount</span><span class="sxs-lookup"><span data-stu-id="d09db-122">readCount</span></span>         | <span data-ttu-id="d09db-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d09db-123">Int64</span></span>             |
| <span data-ttu-id="d09db-124">likedCount</span><span class="sxs-lookup"><span data-stu-id="d09db-124">likedCount</span></span>        | <span data-ttu-id="d09db-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d09db-125">Int64</span></span>             |
| <span data-ttu-id="d09db-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="d09db-126">assignedProducts</span></span>  | <span data-ttu-id="d09db-127">String collection</span><span class="sxs-lookup"><span data-stu-id="d09db-127">String collection</span></span> |
| <span data-ttu-id="d09db-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d09db-128">reportPeriod</span></span>      | <span data-ttu-id="d09db-129">String</span><span class="sxs-lookup"><span data-stu-id="d09db-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="d09db-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d09db-130">JSON representation</span></span>

<span data-ttu-id="d09db-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d09db-131">The following is a JSON representation of the resource.</span></span>

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


