---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 4b80ebc24aa45be0368dbb59d6d3e99e7adacc8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046363"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="67bf4-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="67bf4-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="67bf4-104">属性</span><span class="sxs-lookup"><span data-stu-id="67bf4-104">Properties</span></span>

| <span data-ttu-id="67bf4-105">属性</span><span class="sxs-lookup"><span data-stu-id="67bf4-105">Property</span></span>                | <span data-ttu-id="67bf4-106">类型</span><span class="sxs-lookup"><span data-stu-id="67bf4-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="67bf4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="67bf4-107">reportRefreshDate</span></span>       | <span data-ttu-id="67bf4-108">日期</span><span class="sxs-lookup"><span data-stu-id="67bf4-108">Date</span></span>    |
| <span data-ttu-id="67bf4-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="67bf4-109">siteUrl</span></span>                 | <span data-ttu-id="67bf4-110">字符串</span><span class="sxs-lookup"><span data-stu-id="67bf4-110">String</span></span>  |
| <span data-ttu-id="67bf4-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="67bf4-111">ownerDisplayName</span></span>        | <span data-ttu-id="67bf4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="67bf4-112">String</span></span>  |
| <span data-ttu-id="67bf4-113">被</span><span class="sxs-lookup"><span data-stu-id="67bf4-113">isDeleted</span></span>               | <span data-ttu-id="67bf4-114">布尔</span><span class="sxs-lookup"><span data-stu-id="67bf4-114">Boolean</span></span> |
| <span data-ttu-id="67bf4-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="67bf4-115">lastActivityDate</span></span>        | <span data-ttu-id="67bf4-116">日期</span><span class="sxs-lookup"><span data-stu-id="67bf4-116">Date</span></span>    |
| <span data-ttu-id="67bf4-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="67bf4-117">fileCount</span></span>               | <span data-ttu-id="67bf4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="67bf4-118">Int64</span></span>   |
| <span data-ttu-id="67bf4-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="67bf4-119">activeFileCount</span></span>         | <span data-ttu-id="67bf4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="67bf4-120">Int64</span></span>   |
| <span data-ttu-id="67bf4-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="67bf4-121">storageUsedInBytes</span></span>      | <span data-ttu-id="67bf4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="67bf4-122">Int64</span></span>   |
| <span data-ttu-id="67bf4-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="67bf4-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="67bf4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="67bf4-124">Int64</span></span>   |
| <span data-ttu-id="67bf4-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="67bf4-125">reportPeriod</span></span>            | <span data-ttu-id="67bf4-126">String</span><span class="sxs-lookup"><span data-stu-id="67bf4-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="67bf4-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="67bf4-127">JSON representation</span></span>

<span data-ttu-id="67bf4-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67bf4-128">The following is a JSON representation of the resource.</span></span>

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
