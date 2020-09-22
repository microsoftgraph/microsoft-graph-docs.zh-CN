---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 24f6b9da0fb4e4a141872bd00b423b799b880aa6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048860"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="82f2c-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="82f2c-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="82f2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82f2c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="82f2c-105">属性</span><span class="sxs-lookup"><span data-stu-id="82f2c-105">Properties</span></span>

| <span data-ttu-id="82f2c-106">属性</span><span class="sxs-lookup"><span data-stu-id="82f2c-106">Property</span></span>                  | <span data-ttu-id="82f2c-107">类型</span><span class="sxs-lookup"><span data-stu-id="82f2c-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="82f2c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="82f2c-108">reportRefreshDate</span></span>         | <span data-ttu-id="82f2c-109">日期</span><span class="sxs-lookup"><span data-stu-id="82f2c-109">Date</span></span>              |
| <span data-ttu-id="82f2c-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="82f2c-110">userPrincipalName</span></span>         | <span data-ttu-id="82f2c-111">String</span><span class="sxs-lookup"><span data-stu-id="82f2c-111">String</span></span>            |
| <span data-ttu-id="82f2c-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="82f2c-112">isDeleted</span></span>                 | <span data-ttu-id="82f2c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="82f2c-113">Boolean</span></span>           |
| <span data-ttu-id="82f2c-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="82f2c-114">deletedDate</span></span>               | <span data-ttu-id="82f2c-115">日期</span><span class="sxs-lookup"><span data-stu-id="82f2c-115">Date</span></span>              |
| <span data-ttu-id="82f2c-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="82f2c-116">lastActivityDate</span></span>          | <span data-ttu-id="82f2c-117">日期</span><span class="sxs-lookup"><span data-stu-id="82f2c-117">Date</span></span>              |
| <span data-ttu-id="82f2c-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="82f2c-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="82f2c-119">Int64</span><span class="sxs-lookup"><span data-stu-id="82f2c-119">Int64</span></span>             |
| <span data-ttu-id="82f2c-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="82f2c-120">syncedFileCount</span></span>           | <span data-ttu-id="82f2c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="82f2c-121">Int64</span></span>             |
| <span data-ttu-id="82f2c-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="82f2c-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="82f2c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="82f2c-123">Int64</span></span>             |
| <span data-ttu-id="82f2c-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="82f2c-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="82f2c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="82f2c-125">Int64</span></span>             |
| <span data-ttu-id="82f2c-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="82f2c-126">assignedProducts</span></span>          | <span data-ttu-id="82f2c-127">String 集合</span><span class="sxs-lookup"><span data-stu-id="82f2c-127">String collection</span></span> |
| <span data-ttu-id="82f2c-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="82f2c-128">reportPeriod</span></span>              | <span data-ttu-id="82f2c-129">String</span><span class="sxs-lookup"><span data-stu-id="82f2c-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="82f2c-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82f2c-130">JSON representation</span></span>

<span data-ttu-id="82f2c-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82f2c-131">The following is a JSON representation of the resource.</span></span>

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


