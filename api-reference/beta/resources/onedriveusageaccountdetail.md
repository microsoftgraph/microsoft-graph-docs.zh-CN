---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 594339072c683b053ddeb637b6f401bae2aed322
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812069"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="0b54e-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b54e-103">oneDriveUsageAccountDetail resource type</span></span>

<span data-ttu-id="0b54e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b54e-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0b54e-105">属性</span><span class="sxs-lookup"><span data-stu-id="0b54e-105">Properties</span></span>

| <span data-ttu-id="0b54e-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b54e-106">Property</span></span>                | <span data-ttu-id="0b54e-107">类型</span><span class="sxs-lookup"><span data-stu-id="0b54e-107">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="0b54e-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0b54e-108">reportRefreshDate</span></span>       | <span data-ttu-id="0b54e-109">日期</span><span class="sxs-lookup"><span data-stu-id="0b54e-109">Date</span></span>    |
| <span data-ttu-id="0b54e-110">siteUrl</span><span class="sxs-lookup"><span data-stu-id="0b54e-110">siteUrl</span></span>                 | <span data-ttu-id="0b54e-111">String</span><span class="sxs-lookup"><span data-stu-id="0b54e-111">String</span></span>  |
| <span data-ttu-id="0b54e-112">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="0b54e-112">ownerDisplayName</span></span>        | <span data-ttu-id="0b54e-113">String</span><span class="sxs-lookup"><span data-stu-id="0b54e-113">String</span></span>  |
| <span data-ttu-id="0b54e-114">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b54e-114">ownerPrincipalName</span></span>      | <span data-ttu-id="0b54e-115">String</span><span class="sxs-lookup"><span data-stu-id="0b54e-115">String</span></span>  |
| <span data-ttu-id="0b54e-116">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0b54e-116">isDeleted</span></span>               | <span data-ttu-id="0b54e-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="0b54e-117">Boolean</span></span> |
| <span data-ttu-id="0b54e-118">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0b54e-118">lastActivityDate</span></span>        | <span data-ttu-id="0b54e-119">日期</span><span class="sxs-lookup"><span data-stu-id="0b54e-119">Date</span></span>    |
| <span data-ttu-id="0b54e-120">fileCount</span><span class="sxs-lookup"><span data-stu-id="0b54e-120">fileCount</span></span>               | <span data-ttu-id="0b54e-121">Int64</span><span class="sxs-lookup"><span data-stu-id="0b54e-121">Int64</span></span>   |
| <span data-ttu-id="0b54e-122">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="0b54e-122">activeFileCount</span></span>         | <span data-ttu-id="0b54e-123">Int64</span><span class="sxs-lookup"><span data-stu-id="0b54e-123">Int64</span></span>   |
| <span data-ttu-id="0b54e-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="0b54e-124">storageUsedInBytes</span></span>      | <span data-ttu-id="0b54e-125">Int64</span><span class="sxs-lookup"><span data-stu-id="0b54e-125">Int64</span></span>   |
| <span data-ttu-id="0b54e-126">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="0b54e-126">storageAllocatedInBytes</span></span> | <span data-ttu-id="0b54e-127">Int64</span><span class="sxs-lookup"><span data-stu-id="0b54e-127">Int64</span></span>   |
| <span data-ttu-id="0b54e-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0b54e-128">reportPeriod</span></span>            | <span data-ttu-id="0b54e-129">String</span><span class="sxs-lookup"><span data-stu-id="0b54e-129">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0b54e-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b54e-130">JSON representation</span></span>

<span data-ttu-id="0b54e-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b54e-131">The following is a JSON representation of the resource.</span></span>

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
