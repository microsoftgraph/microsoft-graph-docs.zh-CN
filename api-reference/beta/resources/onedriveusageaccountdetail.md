---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: bcf75fad8c39a543e69fc378546a2621f24eaeab
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2019
ms.locfileid: "34344925"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="30614-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="30614-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="30614-104">属性</span><span class="sxs-lookup"><span data-stu-id="30614-104">Properties</span></span>

| <span data-ttu-id="30614-105">属性</span><span class="sxs-lookup"><span data-stu-id="30614-105">Property</span></span>                | <span data-ttu-id="30614-106">类型</span><span class="sxs-lookup"><span data-stu-id="30614-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="30614-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="30614-107">reportRefreshDate</span></span>       | <span data-ttu-id="30614-108">日期</span><span class="sxs-lookup"><span data-stu-id="30614-108">Date</span></span>    |
| <span data-ttu-id="30614-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="30614-109">siteUrl</span></span>                 | <span data-ttu-id="30614-110">String</span><span class="sxs-lookup"><span data-stu-id="30614-110">String</span></span>  |
| <span data-ttu-id="30614-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="30614-111">ownerDisplayName</span></span>        | <span data-ttu-id="30614-112">String</span><span class="sxs-lookup"><span data-stu-id="30614-112">String</span></span>  |
| <span data-ttu-id="30614-113">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="30614-113">ownerPrincipalName</span></span>      | <span data-ttu-id="30614-114">String</span><span class="sxs-lookup"><span data-stu-id="30614-114">String</span></span>  |
| <span data-ttu-id="30614-115">isDeleted</span><span class="sxs-lookup"><span data-stu-id="30614-115">isDeleted</span></span>               | <span data-ttu-id="30614-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="30614-116">Boolean</span></span> |
| <span data-ttu-id="30614-117">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="30614-117">lastActivityDate</span></span>        | <span data-ttu-id="30614-118">日期</span><span class="sxs-lookup"><span data-stu-id="30614-118">Date</span></span>    |
| <span data-ttu-id="30614-119">fileCount</span><span class="sxs-lookup"><span data-stu-id="30614-119">fileCount</span></span>               | <span data-ttu-id="30614-120">Int64</span><span class="sxs-lookup"><span data-stu-id="30614-120">Int64</span></span>   |
| <span data-ttu-id="30614-121">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="30614-121">activeFileCount</span></span>         | <span data-ttu-id="30614-122">Int64</span><span class="sxs-lookup"><span data-stu-id="30614-122">Int64</span></span>   |
| <span data-ttu-id="30614-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="30614-123">storageUsedInBytes</span></span>      | <span data-ttu-id="30614-124">Int64</span><span class="sxs-lookup"><span data-stu-id="30614-124">Int64</span></span>   |
| <span data-ttu-id="30614-125">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="30614-125">storageAllocatedInBytes</span></span> | <span data-ttu-id="30614-126">Int64</span><span class="sxs-lookup"><span data-stu-id="30614-126">Int64</span></span>   |
| <span data-ttu-id="30614-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="30614-127">reportPeriod</span></span>            | <span data-ttu-id="30614-128">String</span><span class="sxs-lookup"><span data-stu-id="30614-128">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="30614-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30614-129">JSON representation</span></span>

<span data-ttu-id="30614-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30614-130">The following is a JSON representation of the resource.</span></span>

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
