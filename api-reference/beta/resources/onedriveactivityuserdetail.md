---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: c61db94678ed50e6cc93f123a506ce262616a1ab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966480"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="a0f96-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0f96-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a0f96-104">属性</span><span class="sxs-lookup"><span data-stu-id="a0f96-104">Properties</span></span>

| <span data-ttu-id="a0f96-105">属性</span><span class="sxs-lookup"><span data-stu-id="a0f96-105">Property</span></span>                  | <span data-ttu-id="a0f96-106">类型</span><span class="sxs-lookup"><span data-stu-id="a0f96-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="a0f96-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a0f96-107">reportRefreshDate</span></span>         | <span data-ttu-id="a0f96-108">日期</span><span class="sxs-lookup"><span data-stu-id="a0f96-108">Date</span></span>              |
| <span data-ttu-id="a0f96-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a0f96-109">userPrincipalName</span></span>         | <span data-ttu-id="a0f96-110">String</span><span class="sxs-lookup"><span data-stu-id="a0f96-110">String</span></span>            |
| <span data-ttu-id="a0f96-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a0f96-111">isDeleted</span></span>                 | <span data-ttu-id="a0f96-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0f96-112">Boolean</span></span>           |
| <span data-ttu-id="a0f96-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="a0f96-113">deletedDate</span></span>               | <span data-ttu-id="a0f96-114">日期</span><span class="sxs-lookup"><span data-stu-id="a0f96-114">Date</span></span>              |
| <span data-ttu-id="a0f96-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a0f96-115">lastActivityDate</span></span>          | <span data-ttu-id="a0f96-116">日期</span><span class="sxs-lookup"><span data-stu-id="a0f96-116">Date</span></span>              |
| <span data-ttu-id="a0f96-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="a0f96-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="a0f96-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a0f96-118">Int64</span></span>             |
| <span data-ttu-id="a0f96-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="a0f96-119">syncedFileCount</span></span>           | <span data-ttu-id="a0f96-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a0f96-120">Int64</span></span>             |
| <span data-ttu-id="a0f96-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a0f96-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="a0f96-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a0f96-122">Int64</span></span>             |
| <span data-ttu-id="a0f96-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="a0f96-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="a0f96-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a0f96-124">Int64</span></span>             |
| <span data-ttu-id="a0f96-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="a0f96-125">assignedProducts</span></span>          | <span data-ttu-id="a0f96-126">String collection</span><span class="sxs-lookup"><span data-stu-id="a0f96-126">String collection</span></span> |
| <span data-ttu-id="a0f96-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a0f96-127">reportPeriod</span></span>              | <span data-ttu-id="a0f96-128">String</span><span class="sxs-lookup"><span data-stu-id="a0f96-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="a0f96-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0f96-129">JSON representation</span></span>

<span data-ttu-id="a0f96-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0f96-130">The following is a JSON representation of the resource.</span></span>

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
