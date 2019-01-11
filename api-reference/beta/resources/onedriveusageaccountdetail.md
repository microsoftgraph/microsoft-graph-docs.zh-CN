---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 92695f509302ede4b3ce64320e8f4ed42418f7e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842607"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="a788f-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="a788f-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a788f-104">属性</span><span class="sxs-lookup"><span data-stu-id="a788f-104">Properties</span></span>

| <span data-ttu-id="a788f-105">属性</span><span class="sxs-lookup"><span data-stu-id="a788f-105">Property</span></span>                | <span data-ttu-id="a788f-106">类型</span><span class="sxs-lookup"><span data-stu-id="a788f-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="a788f-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a788f-107">reportRefreshDate</span></span>       | <span data-ttu-id="a788f-108">日期</span><span class="sxs-lookup"><span data-stu-id="a788f-108">Date</span></span>    |
| <span data-ttu-id="a788f-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="a788f-109">siteUrl</span></span>                 | <span data-ttu-id="a788f-110">字符串</span><span class="sxs-lookup"><span data-stu-id="a788f-110">String</span></span>  |
| <span data-ttu-id="a788f-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="a788f-111">ownerDisplayName</span></span>        | <span data-ttu-id="a788f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a788f-112">String</span></span>  |
| <span data-ttu-id="a788f-113">被</span><span class="sxs-lookup"><span data-stu-id="a788f-113">isDeleted</span></span>               | <span data-ttu-id="a788f-114">布尔</span><span class="sxs-lookup"><span data-stu-id="a788f-114">Boolean</span></span> |
| <span data-ttu-id="a788f-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a788f-115">lastActivityDate</span></span>        | <span data-ttu-id="a788f-116">日期</span><span class="sxs-lookup"><span data-stu-id="a788f-116">Date</span></span>    |
| <span data-ttu-id="a788f-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="a788f-117">fileCount</span></span>               | <span data-ttu-id="a788f-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a788f-118">Int64</span></span>   |
| <span data-ttu-id="a788f-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="a788f-119">activeFileCount</span></span>         | <span data-ttu-id="a788f-120">Int64</span><span class="sxs-lookup"><span data-stu-id="a788f-120">Int64</span></span>   |
| <span data-ttu-id="a788f-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="a788f-121">storageUsedInBytes</span></span>      | <span data-ttu-id="a788f-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a788f-122">Int64</span></span>   |
| <span data-ttu-id="a788f-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="a788f-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="a788f-124">Int64</span><span class="sxs-lookup"><span data-stu-id="a788f-124">Int64</span></span>   |
| <span data-ttu-id="a788f-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a788f-125">reportPeriod</span></span>            | <span data-ttu-id="a788f-126">String</span><span class="sxs-lookup"><span data-stu-id="a788f-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="a788f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a788f-127">JSON representation</span></span>

<span data-ttu-id="a788f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a788f-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteUrl": "String", 
  "ownerDisplayName": "String", 
  "isDeleted": true, 
  "lastActivityDate": "Date", 
  "fileCount": 1024, 
  "activeFileCount": 1024, 
  "storageUsedInBytes": 1024, 
  "storageAllocatedInBytes": 1024, 
  "reportPeriod": "String"
}
```
