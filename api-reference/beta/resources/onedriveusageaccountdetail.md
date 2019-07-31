---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: cc80110a2f8f755ef984b2f993ea660798a86743
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966466"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="4bebd-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="4bebd-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="4bebd-104">属性</span><span class="sxs-lookup"><span data-stu-id="4bebd-104">Properties</span></span>

| <span data-ttu-id="4bebd-105">属性</span><span class="sxs-lookup"><span data-stu-id="4bebd-105">Property</span></span>                | <span data-ttu-id="4bebd-106">类型</span><span class="sxs-lookup"><span data-stu-id="4bebd-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="4bebd-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="4bebd-107">reportRefreshDate</span></span>       | <span data-ttu-id="4bebd-108">日期</span><span class="sxs-lookup"><span data-stu-id="4bebd-108">Date</span></span>    |
| <span data-ttu-id="4bebd-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="4bebd-109">siteUrl</span></span>                 | <span data-ttu-id="4bebd-110">String</span><span class="sxs-lookup"><span data-stu-id="4bebd-110">String</span></span>  |
| <span data-ttu-id="4bebd-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="4bebd-111">ownerDisplayName</span></span>        | <span data-ttu-id="4bebd-112">String</span><span class="sxs-lookup"><span data-stu-id="4bebd-112">String</span></span>  |
| <span data-ttu-id="4bebd-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4bebd-113">ownerPrincipalName</span></span>      | <span data-ttu-id="4bebd-114">String</span><span class="sxs-lookup"><span data-stu-id="4bebd-114">String</span></span>  |
| <span data-ttu-id="4bebd-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="4bebd-115">isDeleted</span></span>               | <span data-ttu-id="4bebd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4bebd-116">Boolean</span></span> |
| <span data-ttu-id="4bebd-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="4bebd-117">lastActivityDate</span></span>        | <span data-ttu-id="4bebd-118">日期</span><span class="sxs-lookup"><span data-stu-id="4bebd-118">Date</span></span>    |
| <span data-ttu-id="4bebd-119">fileCount</span><span class="sxs-lookup"><span data-stu-id="4bebd-119">fileCount</span></span>               | <span data-ttu-id="4bebd-120">Int64</span><span class="sxs-lookup"><span data-stu-id="4bebd-120">Int64</span></span>   |
| <span data-ttu-id="4bebd-121">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="4bebd-121">activeFileCount</span></span>         | <span data-ttu-id="4bebd-122">Int64</span><span class="sxs-lookup"><span data-stu-id="4bebd-122">Int64</span></span>   |
| <span data-ttu-id="4bebd-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="4bebd-123">storageUsedInBytes</span></span>      | <span data-ttu-id="4bebd-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4bebd-124">Int64</span></span>   |
| <span data-ttu-id="4bebd-125">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="4bebd-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="4bebd-126">Int64</span><span class="sxs-lookup"><span data-stu-id="4bebd-126">Int64</span></span>   |
| <span data-ttu-id="4bebd-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="4bebd-127">reportPeriod</span></span>            | <span data-ttu-id="4bebd-128">String</span><span class="sxs-lookup"><span data-stu-id="4bebd-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="4bebd-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4bebd-129">JSON representation</span></span>

<span data-ttu-id="4bebd-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4bebd-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "ownerPrincipalName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
