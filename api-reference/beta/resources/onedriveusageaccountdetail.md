---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563544"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="29622-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="29622-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="29622-104">属性</span><span class="sxs-lookup"><span data-stu-id="29622-104">Properties</span></span>

| <span data-ttu-id="29622-105">属性</span><span class="sxs-lookup"><span data-stu-id="29622-105">Property</span></span>                | <span data-ttu-id="29622-106">类型</span><span class="sxs-lookup"><span data-stu-id="29622-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="29622-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="29622-107">reportRefreshDate</span></span>       | <span data-ttu-id="29622-108">Date</span><span class="sxs-lookup"><span data-stu-id="29622-108">Date</span></span>    |
| <span data-ttu-id="29622-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="29622-109">siteUrl</span></span>                 | <span data-ttu-id="29622-110">String</span><span class="sxs-lookup"><span data-stu-id="29622-110">String</span></span>  |
| <span data-ttu-id="29622-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="29622-111">ownerDisplayName</span></span>        | <span data-ttu-id="29622-112">String</span><span class="sxs-lookup"><span data-stu-id="29622-112">String</span></span>  |
| <span data-ttu-id="29622-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="29622-113">isDeleted</span></span>               | <span data-ttu-id="29622-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="29622-114">Boolean</span></span> |
| <span data-ttu-id="29622-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="29622-115">lastActivityDate</span></span>        | <span data-ttu-id="29622-116">Date</span><span class="sxs-lookup"><span data-stu-id="29622-116">Date</span></span>    |
| <span data-ttu-id="29622-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="29622-117">fileCount</span></span>               | <span data-ttu-id="29622-118">Int64</span><span class="sxs-lookup"><span data-stu-id="29622-118">Int64</span></span>   |
| <span data-ttu-id="29622-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="29622-119">activeFileCount</span></span>         | <span data-ttu-id="29622-120">Int64</span><span class="sxs-lookup"><span data-stu-id="29622-120">Int64</span></span>   |
| <span data-ttu-id="29622-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="29622-121">storageUsedInBytes</span></span>      | <span data-ttu-id="29622-122">Int64</span><span class="sxs-lookup"><span data-stu-id="29622-122">Int64</span></span>   |
| <span data-ttu-id="29622-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="29622-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="29622-124">Int64</span><span class="sxs-lookup"><span data-stu-id="29622-124">Int64</span></span>   |
| <span data-ttu-id="29622-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="29622-125">reportPeriod</span></span>            | <span data-ttu-id="29622-126">String</span><span class="sxs-lookup"><span data-stu-id="29622-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="29622-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29622-127">JSON representation</span></span>

<span data-ttu-id="29622-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29622-128">The following is a JSON representation of the resource.</span></span>

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
