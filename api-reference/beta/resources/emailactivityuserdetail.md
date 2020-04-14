---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 54efe4d3a24a0409e8daa2ebde6d4aff4b729118
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440567"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="cc3d3-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc3d3-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="cc3d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc3d3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="cc3d3-105">属性</span><span class="sxs-lookup"><span data-stu-id="cc3d3-105">Properties</span></span>

| <span data-ttu-id="cc3d3-106">属性</span><span class="sxs-lookup"><span data-stu-id="cc3d3-106">Property</span></span>          | <span data-ttu-id="cc3d3-107">类型</span><span class="sxs-lookup"><span data-stu-id="cc3d3-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="cc3d3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cc3d3-108">reportRefreshDate</span></span> | <span data-ttu-id="cc3d3-109">日期</span><span class="sxs-lookup"><span data-stu-id="cc3d3-109">Date</span></span>              |
| <span data-ttu-id="cc3d3-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cc3d3-110">userPrincipalName</span></span> | <span data-ttu-id="cc3d3-111">String</span><span class="sxs-lookup"><span data-stu-id="cc3d3-111">String</span></span>            |
| <span data-ttu-id="cc3d3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="cc3d3-112">displayName</span></span>       | <span data-ttu-id="cc3d3-113">String</span><span class="sxs-lookup"><span data-stu-id="cc3d3-113">String</span></span>            |
| <span data-ttu-id="cc3d3-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="cc3d3-114">isDeleted</span></span>         | <span data-ttu-id="cc3d3-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3d3-115">Boolean</span></span>           |
| <span data-ttu-id="cc3d3-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="cc3d3-116">deletedDate</span></span>       | <span data-ttu-id="cc3d3-117">日期</span><span class="sxs-lookup"><span data-stu-id="cc3d3-117">Date</span></span>              |
| <span data-ttu-id="cc3d3-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="cc3d3-118">lastActivityDate</span></span>  | <span data-ttu-id="cc3d3-119">日期</span><span class="sxs-lookup"><span data-stu-id="cc3d3-119">Date</span></span>              |
| <span data-ttu-id="cc3d3-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="cc3d3-120">sendCount</span></span>         | <span data-ttu-id="cc3d3-121">Int64</span><span class="sxs-lookup"><span data-stu-id="cc3d3-121">Int64</span></span>             |
| <span data-ttu-id="cc3d3-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="cc3d3-122">receiveCount</span></span>      | <span data-ttu-id="cc3d3-123">Int64</span><span class="sxs-lookup"><span data-stu-id="cc3d3-123">Int64</span></span>             |
| <span data-ttu-id="cc3d3-124">readCount</span><span class="sxs-lookup"><span data-stu-id="cc3d3-124">readCount</span></span>         | <span data-ttu-id="cc3d3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="cc3d3-125">Int64</span></span>             |
| <span data-ttu-id="cc3d3-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="cc3d3-126">assignedProducts</span></span>  | <span data-ttu-id="cc3d3-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="cc3d3-127">String collection</span></span> |
| <span data-ttu-id="cc3d3-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cc3d3-128">reportPeriod</span></span>      | <span data-ttu-id="cc3d3-129">String</span><span class="sxs-lookup"><span data-stu-id="cc3d3-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="cc3d3-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc3d3-130">JSON representation</span></span>

<span data-ttu-id="cc3d3-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc3d3-131">The following is a JSON representation of the resource.</span></span>

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
