---
title: emailActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: c664cb4a381cf2ebe3de9bd9ca53719786b94405
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499566"
---
# <a name="emailactivityuserdetail-resource-type"></a><span data-ttu-id="70e06-103">emailActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="70e06-103">emailActivityUserDetail resource type</span></span>

<span data-ttu-id="70e06-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="70e06-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="70e06-105">属性</span><span class="sxs-lookup"><span data-stu-id="70e06-105">Properties</span></span>

| <span data-ttu-id="70e06-106">属性</span><span class="sxs-lookup"><span data-stu-id="70e06-106">Property</span></span>          | <span data-ttu-id="70e06-107">类型</span><span class="sxs-lookup"><span data-stu-id="70e06-107">Type</span></span>              |
| :---------------- | :---------------- |
| <span data-ttu-id="70e06-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="70e06-108">reportRefreshDate</span></span> | <span data-ttu-id="70e06-109">日期</span><span class="sxs-lookup"><span data-stu-id="70e06-109">Date</span></span>              |
| <span data-ttu-id="70e06-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70e06-110">userPrincipalName</span></span> | <span data-ttu-id="70e06-111">String</span><span class="sxs-lookup"><span data-stu-id="70e06-111">String</span></span>            |
| <span data-ttu-id="70e06-112">displayName</span><span class="sxs-lookup"><span data-stu-id="70e06-112">displayName</span></span>       | <span data-ttu-id="70e06-113">String</span><span class="sxs-lookup"><span data-stu-id="70e06-113">String</span></span>            |
| <span data-ttu-id="70e06-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="70e06-114">isDeleted</span></span>         | <span data-ttu-id="70e06-115">布尔</span><span class="sxs-lookup"><span data-stu-id="70e06-115">Boolean</span></span>           |
| <span data-ttu-id="70e06-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="70e06-116">deletedDate</span></span>       | <span data-ttu-id="70e06-117">日期</span><span class="sxs-lookup"><span data-stu-id="70e06-117">Date</span></span>              |
| <span data-ttu-id="70e06-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="70e06-118">lastActivityDate</span></span>  | <span data-ttu-id="70e06-119">日期</span><span class="sxs-lookup"><span data-stu-id="70e06-119">Date</span></span>              |
| <span data-ttu-id="70e06-120">sendCount</span><span class="sxs-lookup"><span data-stu-id="70e06-120">sendCount</span></span>         | <span data-ttu-id="70e06-121">Int64</span><span class="sxs-lookup"><span data-stu-id="70e06-121">Int64</span></span>             |
| <span data-ttu-id="70e06-122">receiveCount</span><span class="sxs-lookup"><span data-stu-id="70e06-122">receiveCount</span></span>      | <span data-ttu-id="70e06-123">Int64</span><span class="sxs-lookup"><span data-stu-id="70e06-123">Int64</span></span>             |
| <span data-ttu-id="70e06-124">readCount</span><span class="sxs-lookup"><span data-stu-id="70e06-124">readCount</span></span>         | <span data-ttu-id="70e06-125">Int64</span><span class="sxs-lookup"><span data-stu-id="70e06-125">Int64</span></span>             |
| <span data-ttu-id="70e06-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="70e06-126">assignedProducts</span></span>  | <span data-ttu-id="70e06-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="70e06-127">String collection</span></span> |
| <span data-ttu-id="70e06-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="70e06-128">reportPeriod</span></span>      | <span data-ttu-id="70e06-129">String</span><span class="sxs-lookup"><span data-stu-id="70e06-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="70e06-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70e06-130">JSON representation</span></span>

<span data-ttu-id="70e06-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70e06-131">The following is a JSON representation of the resource.</span></span>

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
