---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 6e355e1f71d493b30ffb2fe41816208dfe4816e9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039284"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="73ec5-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="73ec5-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="73ec5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73ec5-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="73ec5-105">属性</span><span class="sxs-lookup"><span data-stu-id="73ec5-105">Properties</span></span>

| <span data-ttu-id="73ec5-106">属性</span><span class="sxs-lookup"><span data-stu-id="73ec5-106">Property</span></span>                | <span data-ttu-id="73ec5-107">类型</span><span class="sxs-lookup"><span data-stu-id="73ec5-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="73ec5-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="73ec5-108">reportRefreshDate</span></span>       | <span data-ttu-id="73ec5-109">日期</span><span class="sxs-lookup"><span data-stu-id="73ec5-109">Date</span></span>    |
| <span data-ttu-id="73ec5-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="73ec5-110">siteUrl</span></span>                 | <span data-ttu-id="73ec5-111">String</span><span class="sxs-lookup"><span data-stu-id="73ec5-111">String</span></span>  |
| <span data-ttu-id="73ec5-112">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="73ec5-112">ownerDisplayName</span></span>        | <span data-ttu-id="73ec5-113">String</span><span class="sxs-lookup"><span data-stu-id="73ec5-113">String</span></span>  |
| <span data-ttu-id="73ec5-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="73ec5-114">ownerPrincipalName</span></span>      | <span data-ttu-id="73ec5-115">String</span><span class="sxs-lookup"><span data-stu-id="73ec5-115">String</span></span>  |
| <span data-ttu-id="73ec5-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="73ec5-116">isDeleted</span></span>               | <span data-ttu-id="73ec5-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="73ec5-117">Boolean</span></span> |
| <span data-ttu-id="73ec5-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="73ec5-118">lastActivityDate</span></span>        | <span data-ttu-id="73ec5-119">日期</span><span class="sxs-lookup"><span data-stu-id="73ec5-119">Date</span></span>    |
| <span data-ttu-id="73ec5-120">fileCount</span><span class="sxs-lookup"><span data-stu-id="73ec5-120">fileCount</span></span>               | <span data-ttu-id="73ec5-121">Int64</span><span class="sxs-lookup"><span data-stu-id="73ec5-121">Int64</span></span>   |
| <span data-ttu-id="73ec5-122">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="73ec5-122">activeFileCount</span></span>         | <span data-ttu-id="73ec5-123">Int64</span><span class="sxs-lookup"><span data-stu-id="73ec5-123">Int64</span></span>   |
| <span data-ttu-id="73ec5-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="73ec5-124">storageUsedInBytes</span></span>      | <span data-ttu-id="73ec5-125">Int64</span><span class="sxs-lookup"><span data-stu-id="73ec5-125">Int64</span></span>   |
| <span data-ttu-id="73ec5-126">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="73ec5-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="73ec5-127">Int64</span><span class="sxs-lookup"><span data-stu-id="73ec5-127">Int64</span></span>   |
| <span data-ttu-id="73ec5-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="73ec5-128">reportPeriod</span></span>            | <span data-ttu-id="73ec5-129">String</span><span class="sxs-lookup"><span data-stu-id="73ec5-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="73ec5-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73ec5-130">JSON representation</span></span>

<span data-ttu-id="73ec5-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73ec5-131">The following is a JSON representation of the resource.</span></span>

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


