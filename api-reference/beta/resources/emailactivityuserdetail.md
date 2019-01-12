---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b871bf5dbaedd961fad09bf97be868f46e7430a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938305"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="6f712-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="6f712-103">emailActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6f712-104">属性</span><span class="sxs-lookup"><span data-stu-id="6f712-104">Properties</span></span>

| <span data-ttu-id="6f712-105">属性</span><span class="sxs-lookup"><span data-stu-id="6f712-105">Property</span></span>          | <span data-ttu-id="6f712-106">类型</span><span class="sxs-lookup"><span data-stu-id="6f712-106">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="6f712-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6f712-107">reportRefreshDate</span></span> | <span data-ttu-id="6f712-108">日期</span><span class="sxs-lookup"><span data-stu-id="6f712-108">Date</span></span>              |
| <span data-ttu-id="6f712-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6f712-109">userPrincipalName</span></span> | <span data-ttu-id="6f712-110">字符串</span><span class="sxs-lookup"><span data-stu-id="6f712-110">String</span></span>            |
| <span data-ttu-id="6f712-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6f712-111">displayName</span></span>       | <span data-ttu-id="6f712-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6f712-112">String</span></span>            |
| <span data-ttu-id="6f712-113">被</span><span class="sxs-lookup"><span data-stu-id="6f712-113">isDeleted</span></span>         | <span data-ttu-id="6f712-114">布尔</span><span class="sxs-lookup"><span data-stu-id="6f712-114">Boolean</span></span>           |
| <span data-ttu-id="6f712-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6f712-115">deletedDate</span></span>       | <span data-ttu-id="6f712-116">日期</span><span class="sxs-lookup"><span data-stu-id="6f712-116">Date</span></span>              |
| <span data-ttu-id="6f712-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6f712-117">lastActivityDate</span></span>  | <span data-ttu-id="6f712-118">日期</span><span class="sxs-lookup"><span data-stu-id="6f712-118">Date</span></span>              |
| <span data-ttu-id="6f712-119">sendCount</span><span class="sxs-lookup"><span data-stu-id="6f712-119">sendCount</span></span>         | <span data-ttu-id="6f712-120">Int64</span><span class="sxs-lookup"><span data-stu-id="6f712-120">Int64</span></span>             |
| <span data-ttu-id="6f712-121">receiveCount</span><span class="sxs-lookup"><span data-stu-id="6f712-121">receiveCount</span></span>      | <span data-ttu-id="6f712-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6f712-122">Int64</span></span>             |
| <span data-ttu-id="6f712-123">readCount</span><span class="sxs-lookup"><span data-stu-id="6f712-123">readCount</span></span>         | <span data-ttu-id="6f712-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6f712-124">Int64</span></span>             |
| <span data-ttu-id="6f712-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="6f712-125">assignedProducts</span></span>  | <span data-ttu-id="6f712-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="6f712-126">String collection</span></span> |
| <span data-ttu-id="6f712-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6f712-127">reportPeriod</span></span>      | <span data-ttu-id="6f712-128">String</span><span class="sxs-lookup"><span data-stu-id="6f712-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="6f712-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f712-129">JSON representation</span></span>

<span data-ttu-id="6f712-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f712-130">The following is a JSON representation of the resource.</span></span>

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
