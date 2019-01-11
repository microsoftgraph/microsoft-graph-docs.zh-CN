---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 2f498c7c9507c4210f12f76d57f62729f84da578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820788"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="c18b4-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c18b4-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c18b4-104">属性</span><span class="sxs-lookup"><span data-stu-id="c18b4-104">Properties</span></span>

| <span data-ttu-id="c18b4-105">属性</span><span class="sxs-lookup"><span data-stu-id="c18b4-105">Property</span></span>                  | <span data-ttu-id="c18b4-106">类型</span><span class="sxs-lookup"><span data-stu-id="c18b4-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="c18b4-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c18b4-107">reportRefreshDate</span></span>         | <span data-ttu-id="c18b4-108">日期</span><span class="sxs-lookup"><span data-stu-id="c18b4-108">Date</span></span>              |
| <span data-ttu-id="c18b4-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c18b4-109">userPrincipalName</span></span>         | <span data-ttu-id="c18b4-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c18b4-110">String</span></span>            |
| <span data-ttu-id="c18b4-111">被</span><span class="sxs-lookup"><span data-stu-id="c18b4-111">isDeleted</span></span>                 | <span data-ttu-id="c18b4-112">布尔</span><span class="sxs-lookup"><span data-stu-id="c18b4-112">Boolean</span></span>           |
| <span data-ttu-id="c18b4-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c18b4-113">deletedDate</span></span>               | <span data-ttu-id="c18b4-114">日期</span><span class="sxs-lookup"><span data-stu-id="c18b4-114">Date</span></span>              |
| <span data-ttu-id="c18b4-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c18b4-115">lastActivityDate</span></span>          | <span data-ttu-id="c18b4-116">日期</span><span class="sxs-lookup"><span data-stu-id="c18b4-116">Date</span></span>              |
| <span data-ttu-id="c18b4-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="c18b4-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="c18b4-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c18b4-118">Int64</span></span>             |
| <span data-ttu-id="c18b4-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="c18b4-119">syncedFileCount</span></span>           | <span data-ttu-id="c18b4-120">Int64</span><span class="sxs-lookup"><span data-stu-id="c18b4-120">Int64</span></span>             |
| <span data-ttu-id="c18b4-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c18b4-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="c18b4-122">Int64</span><span class="sxs-lookup"><span data-stu-id="c18b4-122">Int64</span></span>             |
| <span data-ttu-id="c18b4-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="c18b4-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="c18b4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="c18b4-124">Int64</span></span>             |
| <span data-ttu-id="c18b4-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="c18b4-125">assignedProducts</span></span>          | <span data-ttu-id="c18b4-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="c18b4-126">String collection</span></span> |
| <span data-ttu-id="c18b4-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c18b4-127">reportPeriod</span></span>              | <span data-ttu-id="c18b4-128">String</span><span class="sxs-lookup"><span data-stu-id="c18b4-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="c18b4-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c18b4-129">JSON representation</span></span>

<span data-ttu-id="c18b4-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c18b4-130">The following is a JSON representation of the resource.</span></span>

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
