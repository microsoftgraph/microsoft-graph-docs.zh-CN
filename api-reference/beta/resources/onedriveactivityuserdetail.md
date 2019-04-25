---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 29c9c8b723d4f87fa9858e26906878c973b37b09
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582246"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="bff57-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="bff57-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bff57-104">属性</span><span class="sxs-lookup"><span data-stu-id="bff57-104">Properties</span></span>

| <span data-ttu-id="bff57-105">属性</span><span class="sxs-lookup"><span data-stu-id="bff57-105">Property</span></span>                  | <span data-ttu-id="bff57-106">类型</span><span class="sxs-lookup"><span data-stu-id="bff57-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="bff57-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bff57-107">reportRefreshDate</span></span>         | <span data-ttu-id="bff57-108">Date</span><span class="sxs-lookup"><span data-stu-id="bff57-108">Date</span></span>              |
| <span data-ttu-id="bff57-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bff57-109">userPrincipalName</span></span>         | <span data-ttu-id="bff57-110">String</span><span class="sxs-lookup"><span data-stu-id="bff57-110">String</span></span>            |
| <span data-ttu-id="bff57-111">isDeleted</span><span class="sxs-lookup"><span data-stu-id="bff57-111">isDeleted</span></span>                 | <span data-ttu-id="bff57-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bff57-112">Boolean</span></span>           |
| <span data-ttu-id="bff57-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="bff57-113">deletedDate</span></span>               | <span data-ttu-id="bff57-114">Date</span><span class="sxs-lookup"><span data-stu-id="bff57-114">Date</span></span>              |
| <span data-ttu-id="bff57-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="bff57-115">lastActivityDate</span></span>          | <span data-ttu-id="bff57-116">Date</span><span class="sxs-lookup"><span data-stu-id="bff57-116">Date</span></span>              |
| <span data-ttu-id="bff57-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="bff57-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="bff57-118">Int64</span><span class="sxs-lookup"><span data-stu-id="bff57-118">Int64</span></span>             |
| <span data-ttu-id="bff57-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="bff57-119">syncedFileCount</span></span>           | <span data-ttu-id="bff57-120">Int64</span><span class="sxs-lookup"><span data-stu-id="bff57-120">Int64</span></span>             |
| <span data-ttu-id="bff57-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bff57-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="bff57-122">Int64</span><span class="sxs-lookup"><span data-stu-id="bff57-122">Int64</span></span>             |
| <span data-ttu-id="bff57-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="bff57-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="bff57-124">Int64</span><span class="sxs-lookup"><span data-stu-id="bff57-124">Int64</span></span>             |
| <span data-ttu-id="bff57-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="bff57-125">assignedProducts</span></span>          | <span data-ttu-id="bff57-126">String collection</span><span class="sxs-lookup"><span data-stu-id="bff57-126">String collection</span></span> |
| <span data-ttu-id="bff57-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bff57-127">reportPeriod</span></span>              | <span data-ttu-id="bff57-128">String</span><span class="sxs-lookup"><span data-stu-id="bff57-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="bff57-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bff57-129">JSON representation</span></span>

<span data-ttu-id="bff57-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bff57-130">The following is a JSON representation of the resource.</span></span>

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
