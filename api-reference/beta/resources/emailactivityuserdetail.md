---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 73e743bc6409f762a7898ec8037633c7bc3f00e4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981849"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="067f7-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="067f7-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="067f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="067f7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="067f7-105">属性</span><span class="sxs-lookup"><span data-stu-id="067f7-105">Properties</span></span>

| <span data-ttu-id="067f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="067f7-106">Property</span></span>          | <span data-ttu-id="067f7-107">类型</span><span class="sxs-lookup"><span data-stu-id="067f7-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="067f7-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="067f7-108">reportRefreshDate</span></span> | <span data-ttu-id="067f7-109">日期</span><span class="sxs-lookup"><span data-stu-id="067f7-109">Date</span></span>              |
| <span data-ttu-id="067f7-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="067f7-110">userPrincipalName</span></span> | <span data-ttu-id="067f7-111">String</span><span class="sxs-lookup"><span data-stu-id="067f7-111">String</span></span>            |
| <span data-ttu-id="067f7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="067f7-112">displayName</span></span>       | <span data-ttu-id="067f7-113">String</span><span class="sxs-lookup"><span data-stu-id="067f7-113">String</span></span>            |
| <span data-ttu-id="067f7-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="067f7-114">isDeleted</span></span>         | <span data-ttu-id="067f7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="067f7-115">Boolean</span></span>           |
| <span data-ttu-id="067f7-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="067f7-116">deletedDate</span></span>       | <span data-ttu-id="067f7-117">日期</span><span class="sxs-lookup"><span data-stu-id="067f7-117">Date</span></span>              |
| <span data-ttu-id="067f7-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="067f7-118">lastActivityDate</span></span>  | <span data-ttu-id="067f7-119">日期</span><span class="sxs-lookup"><span data-stu-id="067f7-119">Date</span></span>              |
| <span data-ttu-id="067f7-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="067f7-120">sendCount</span></span>         | <span data-ttu-id="067f7-121">Int64</span><span class="sxs-lookup"><span data-stu-id="067f7-121">Int64</span></span>             |
| <span data-ttu-id="067f7-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="067f7-122">receiveCount</span></span>      | <span data-ttu-id="067f7-123">Int64</span><span class="sxs-lookup"><span data-stu-id="067f7-123">Int64</span></span>             |
| <span data-ttu-id="067f7-124">readCount</span><span class="sxs-lookup"><span data-stu-id="067f7-124">readCount</span></span>         | <span data-ttu-id="067f7-125">Int64</span><span class="sxs-lookup"><span data-stu-id="067f7-125">Int64</span></span>             |
| <span data-ttu-id="067f7-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="067f7-126">assignedProducts</span></span>  | <span data-ttu-id="067f7-127">String collection</span><span class="sxs-lookup"><span data-stu-id="067f7-127">String collection</span></span> |
| <span data-ttu-id="067f7-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="067f7-128">reportPeriod</span></span>      | <span data-ttu-id="067f7-129">String</span><span class="sxs-lookup"><span data-stu-id="067f7-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="067f7-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="067f7-130">JSON representation</span></span>

<span data-ttu-id="067f7-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="067f7-131">The following is a JSON representation of the resource.</span></span>

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


