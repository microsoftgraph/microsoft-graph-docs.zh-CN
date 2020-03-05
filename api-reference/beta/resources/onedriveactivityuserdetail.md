---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 22702a392a76a21951c24667da0e8a1e61c8b36c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522391"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="39da3-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="39da3-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="39da3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="39da3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="39da3-105">属性</span><span class="sxs-lookup"><span data-stu-id="39da3-105">Properties</span></span>

| <span data-ttu-id="39da3-106">属性</span><span class="sxs-lookup"><span data-stu-id="39da3-106">Property</span></span>                  | <span data-ttu-id="39da3-107">类型</span><span class="sxs-lookup"><span data-stu-id="39da3-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="39da3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="39da3-108">reportRefreshDate</span></span>         | <span data-ttu-id="39da3-109">日期</span><span class="sxs-lookup"><span data-stu-id="39da3-109">Date</span></span>              |
| <span data-ttu-id="39da3-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="39da3-110">userPrincipalName</span></span>         | <span data-ttu-id="39da3-111">String</span><span class="sxs-lookup"><span data-stu-id="39da3-111">String</span></span>            |
| <span data-ttu-id="39da3-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="39da3-112">isDeleted</span></span>                 | <span data-ttu-id="39da3-113">布尔</span><span class="sxs-lookup"><span data-stu-id="39da3-113">Boolean</span></span>           |
| <span data-ttu-id="39da3-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="39da3-114">deletedDate</span></span>               | <span data-ttu-id="39da3-115">日期</span><span class="sxs-lookup"><span data-stu-id="39da3-115">Date</span></span>              |
| <span data-ttu-id="39da3-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="39da3-116">lastActivityDate</span></span>          | <span data-ttu-id="39da3-117">日期</span><span class="sxs-lookup"><span data-stu-id="39da3-117">Date</span></span>              |
| <span data-ttu-id="39da3-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="39da3-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="39da3-119">Int64</span><span class="sxs-lookup"><span data-stu-id="39da3-119">Int64</span></span>             |
| <span data-ttu-id="39da3-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="39da3-120">syncedFileCount</span></span>           | <span data-ttu-id="39da3-121">Int64</span><span class="sxs-lookup"><span data-stu-id="39da3-121">Int64</span></span>             |
| <span data-ttu-id="39da3-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="39da3-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="39da3-123">Int64</span><span class="sxs-lookup"><span data-stu-id="39da3-123">Int64</span></span>             |
| <span data-ttu-id="39da3-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="39da3-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="39da3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="39da3-125">Int64</span></span>             |
| <span data-ttu-id="39da3-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="39da3-126">assignedProducts</span></span>          | <span data-ttu-id="39da3-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="39da3-127">String collection</span></span> |
| <span data-ttu-id="39da3-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="39da3-128">reportPeriod</span></span>              | <span data-ttu-id="39da3-129">String</span><span class="sxs-lookup"><span data-stu-id="39da3-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="39da3-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39da3-130">JSON representation</span></span>

<span data-ttu-id="39da3-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39da3-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "lastActivityDate": "Date", 
  "viewedOrEditedFileCount": 1024, 
  "syncedFileCount": 1024, 
  "sharedInternallyFileCount": 1024, 
  "sharedExternallyFileCount": 1024, 
  "assignedProducts": ["String"], 
  "reportPeriod": "String"
}
```
