---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 679ec9b8452d388fe311e67d88bcfffd6fe73d93
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044186"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="86cf6-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="86cf6-103">oneDriveActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="86cf6-104">属性</span><span class="sxs-lookup"><span data-stu-id="86cf6-104">Properties</span></span>

| <span data-ttu-id="86cf6-105">属性</span><span class="sxs-lookup"><span data-stu-id="86cf6-105">Property</span></span>                  | <span data-ttu-id="86cf6-106">类型</span><span class="sxs-lookup"><span data-stu-id="86cf6-106">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="86cf6-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="86cf6-107">reportRefreshDate</span></span>         | <span data-ttu-id="86cf6-108">日期</span><span class="sxs-lookup"><span data-stu-id="86cf6-108">Date</span></span>              |
| <span data-ttu-id="86cf6-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86cf6-109">userPrincipalName</span></span>         | <span data-ttu-id="86cf6-110">字符串</span><span class="sxs-lookup"><span data-stu-id="86cf6-110">String</span></span>            |
| <span data-ttu-id="86cf6-111">被</span><span class="sxs-lookup"><span data-stu-id="86cf6-111">isDeleted</span></span>                 | <span data-ttu-id="86cf6-112">布尔</span><span class="sxs-lookup"><span data-stu-id="86cf6-112">Boolean</span></span>           |
| <span data-ttu-id="86cf6-113">deletedDate</span><span class="sxs-lookup"><span data-stu-id="86cf6-113">deletedDate</span></span>               | <span data-ttu-id="86cf6-114">日期</span><span class="sxs-lookup"><span data-stu-id="86cf6-114">Date</span></span>              |
| <span data-ttu-id="86cf6-115">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="86cf6-115">lastActivityDate</span></span>          | <span data-ttu-id="86cf6-116">日期</span><span class="sxs-lookup"><span data-stu-id="86cf6-116">Date</span></span>              |
| <span data-ttu-id="86cf6-117">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="86cf6-117">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="86cf6-118">Int64</span><span class="sxs-lookup"><span data-stu-id="86cf6-118">Int64</span></span>             |
| <span data-ttu-id="86cf6-119">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="86cf6-119">syncedFileCount</span></span>           | <span data-ttu-id="86cf6-120">Int64</span><span class="sxs-lookup"><span data-stu-id="86cf6-120">Int64</span></span>             |
| <span data-ttu-id="86cf6-121">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="86cf6-121">sharedInternallyFileCount</span></span> | <span data-ttu-id="86cf6-122">Int64</span><span class="sxs-lookup"><span data-stu-id="86cf6-122">Int64</span></span>             |
| <span data-ttu-id="86cf6-123">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="86cf6-123">sharedExternallyFileCount</span></span> | <span data-ttu-id="86cf6-124">Int64</span><span class="sxs-lookup"><span data-stu-id="86cf6-124">Int64</span></span>             |
| <span data-ttu-id="86cf6-125">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="86cf6-125">assignedProducts</span></span>          | <span data-ttu-id="86cf6-126">String 集合</span><span class="sxs-lookup"><span data-stu-id="86cf6-126">String collection</span></span> |
| <span data-ttu-id="86cf6-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="86cf6-127">reportPeriod</span></span>              | <span data-ttu-id="86cf6-128">String</span><span class="sxs-lookup"><span data-stu-id="86cf6-128">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="86cf6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86cf6-129">JSON representation</span></span>

<span data-ttu-id="86cf6-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86cf6-130">The following is a JSON representation of the resource.</span></span>

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
