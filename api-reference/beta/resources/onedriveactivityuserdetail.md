---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948245"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="0a4c1-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a4c1-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0a4c1-104">属性</span><span class="sxs-lookup"><span data-stu-id="0a4c1-104">Properties</span></span>

| <span data-ttu-id="0a4c1-105">属性</span><span class="sxs-lookup"><span data-stu-id="0a4c1-105">Property</span></span>                  | <span data-ttu-id="0a4c1-106">类型</span><span class="sxs-lookup"><span data-stu-id="0a4c1-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="0a4c1-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0a4c1-107">reportRefreshDate</span></span>         | <span data-ttu-id="0a4c1-108">日期</span><span class="sxs-lookup"><span data-stu-id="0a4c1-108">Date</span></span>              |
| <span data-ttu-id="0a4c1-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0a4c1-109">userPrincipalName</span></span>         | <span data-ttu-id="0a4c1-110">字符串</span><span class="sxs-lookup"><span data-stu-id="0a4c1-110">String</span></span>            |
| <span data-ttu-id="0a4c1-111">被</span><span class="sxs-lookup"><span data-stu-id="0a4c1-111">isDeleted</span></span>                 | <span data-ttu-id="0a4c1-112">布尔</span><span class="sxs-lookup"><span data-stu-id="0a4c1-112">Boolean</span></span>           |
| <span data-ttu-id="0a4c1-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="0a4c1-113">deletedDate</span></span>               | <span data-ttu-id="0a4c1-114">日期</span><span class="sxs-lookup"><span data-stu-id="0a4c1-114">Date</span></span>              |
| <span data-ttu-id="0a4c1-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0a4c1-115">lastActivityDate</span></span>          | <span data-ttu-id="0a4c1-116">日期</span><span class="sxs-lookup"><span data-stu-id="0a4c1-116">Date</span></span>              |
| <span data-ttu-id="0a4c1-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="0a4c1-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="0a4c1-118">Int64</span><span class="sxs-lookup"><span data-stu-id="0a4c1-118">Int64</span></span>             |
| <span data-ttu-id="0a4c1-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="0a4c1-119">syncedFileCount</span></span>           | <span data-ttu-id="0a4c1-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0a4c1-120">Int64</span></span>             |
| <span data-ttu-id="0a4c1-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="0a4c1-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="0a4c1-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0a4c1-122">Int64</span></span>             |
| <span data-ttu-id="0a4c1-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="0a4c1-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="0a4c1-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0a4c1-124">Int64</span></span>             |
| <span data-ttu-id="0a4c1-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="0a4c1-125">assignedProducts</span></span>          | <span data-ttu-id="0a4c1-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="0a4c1-126">String collection</span></span> |
| <span data-ttu-id="0a4c1-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0a4c1-127">reportPeriod</span></span>              | <span data-ttu-id="0a4c1-128">String</span><span class="sxs-lookup"><span data-stu-id="0a4c1-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="0a4c1-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a4c1-129">JSON representation</span></span>

<span data-ttu-id="0a4c1-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a4c1-130">The following is a JSON representation of the resource.</span></span>

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
