---
title: oneDriveUsageAccountDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c13e03d1170b0ebbc53394541c4564c60c67e78
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957394"
---
# <a name="onedriveusageaccountdetail-resource-type"></a><span data-ttu-id="56724-103">oneDriveUsageAccountDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="56724-103">oneDriveUsageAccountDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="56724-104">属性</span><span class="sxs-lookup"><span data-stu-id="56724-104">Properties</span></span>

| <span data-ttu-id="56724-105">属性</span><span class="sxs-lookup"><span data-stu-id="56724-105">Property</span></span>                | <span data-ttu-id="56724-106">类型</span><span class="sxs-lookup"><span data-stu-id="56724-106">Type</span></span>    |
| :---------------------- | :------ |
| <span data-ttu-id="56724-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="56724-107">reportRefreshDate</span></span>       | <span data-ttu-id="56724-108">日期</span><span class="sxs-lookup"><span data-stu-id="56724-108">Date</span></span>    |
| <span data-ttu-id="56724-109">siteUrl</span><span class="sxs-lookup"><span data-stu-id="56724-109">siteUrl</span></span>                 | <span data-ttu-id="56724-110">字符串</span><span class="sxs-lookup"><span data-stu-id="56724-110">String</span></span>  |
| <span data-ttu-id="56724-111">ownerDisplayName</span><span class="sxs-lookup"><span data-stu-id="56724-111">ownerDisplayName</span></span>        | <span data-ttu-id="56724-112">字符串</span><span class="sxs-lookup"><span data-stu-id="56724-112">String</span></span>  |
| <span data-ttu-id="56724-113">被</span><span class="sxs-lookup"><span data-stu-id="56724-113">isDeleted</span></span>               | <span data-ttu-id="56724-114">布尔</span><span class="sxs-lookup"><span data-stu-id="56724-114">Boolean</span></span> |
| <span data-ttu-id="56724-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="56724-115">lastActivityDate</span></span>        | <span data-ttu-id="56724-116">日期</span><span class="sxs-lookup"><span data-stu-id="56724-116">Date</span></span>    |
| <span data-ttu-id="56724-117">fileCount</span><span class="sxs-lookup"><span data-stu-id="56724-117">fileCount</span></span>               | <span data-ttu-id="56724-118">Int64</span><span class="sxs-lookup"><span data-stu-id="56724-118">Int64</span></span>   |
| <span data-ttu-id="56724-119">activeFileCount</span><span class="sxs-lookup"><span data-stu-id="56724-119">activeFileCount</span></span>         | <span data-ttu-id="56724-120">Int64</span><span class="sxs-lookup"><span data-stu-id="56724-120">Int64</span></span>   |
| <span data-ttu-id="56724-121">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="56724-121">storageUsedInBytes</span></span>      | <span data-ttu-id="56724-122">Int64</span><span class="sxs-lookup"><span data-stu-id="56724-122">Int64</span></span>   |
| <span data-ttu-id="56724-123">storageAllocatedInBytes</span><span class="sxs-lookup"><span data-stu-id="56724-123">storageAllocatedInBytes</span></span> | <span data-ttu-id="56724-124">Int64</span><span class="sxs-lookup"><span data-stu-id="56724-124">Int64</span></span>   |
| <span data-ttu-id="56724-125">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="56724-125">reportPeriod</span></span>            | <span data-ttu-id="56724-126">String</span><span class="sxs-lookup"><span data-stu-id="56724-126">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="56724-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56724-127">JSON representation</span></span>

<span data-ttu-id="56724-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56724-128">The following is a JSON representation of the resource.</span></span>

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
