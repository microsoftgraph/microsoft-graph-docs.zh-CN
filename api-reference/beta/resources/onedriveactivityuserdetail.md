---
title: oneDriveActivityUserDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 4021d1bdfb9322dbef75264ab88bb8b3a71c20e7
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812146"
---
# <a name="onedriveactivityuserdetail-resource-type"></a><span data-ttu-id="23622-103">oneDriveActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="23622-103">oneDriveActivityUserDetail resource type</span></span>

<span data-ttu-id="23622-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23622-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="23622-105">属性</span><span class="sxs-lookup"><span data-stu-id="23622-105">Properties</span></span>

| <span data-ttu-id="23622-106">属性</span><span class="sxs-lookup"><span data-stu-id="23622-106">Property</span></span>                  | <span data-ttu-id="23622-107">类型</span><span class="sxs-lookup"><span data-stu-id="23622-107">Type</span></span>              |
| :------------------------ | :---------------- |
| <span data-ttu-id="23622-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="23622-108">reportRefreshDate</span></span>         | <span data-ttu-id="23622-109">日期</span><span class="sxs-lookup"><span data-stu-id="23622-109">Date</span></span>              |
| <span data-ttu-id="23622-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23622-110">userPrincipalName</span></span>         | <span data-ttu-id="23622-111">String</span><span class="sxs-lookup"><span data-stu-id="23622-111">String</span></span>            |
| <span data-ttu-id="23622-112">isDeleted</span><span class="sxs-lookup"><span data-stu-id="23622-112">isDeleted</span></span>                 | <span data-ttu-id="23622-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="23622-113">Boolean</span></span>           |
| <span data-ttu-id="23622-114">deletedDate</span><span class="sxs-lookup"><span data-stu-id="23622-114">deletedDate</span></span>               | <span data-ttu-id="23622-115">日期</span><span class="sxs-lookup"><span data-stu-id="23622-115">Date</span></span>              |
| <span data-ttu-id="23622-116">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="23622-116">lastActivityDate</span></span>          | <span data-ttu-id="23622-117">日期</span><span class="sxs-lookup"><span data-stu-id="23622-117">Date</span></span>              |
| <span data-ttu-id="23622-118">viewedOrEditedFileCount</span><span class="sxs-lookup"><span data-stu-id="23622-118">viewedOrEditedFileCount</span></span>   | <span data-ttu-id="23622-119">Int64</span><span class="sxs-lookup"><span data-stu-id="23622-119">Int64</span></span>             |
| <span data-ttu-id="23622-120">syncedFileCount</span><span class="sxs-lookup"><span data-stu-id="23622-120">syncedFileCount</span></span>           | <span data-ttu-id="23622-121">Int64</span><span class="sxs-lookup"><span data-stu-id="23622-121">Int64</span></span>             |
| <span data-ttu-id="23622-122">sharedInternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="23622-122">sharedInternallyFileCount</span></span> | <span data-ttu-id="23622-123">Int64</span><span class="sxs-lookup"><span data-stu-id="23622-123">Int64</span></span>             |
| <span data-ttu-id="23622-124">sharedExternallyFileCount</span><span class="sxs-lookup"><span data-stu-id="23622-124">sharedExternallyFileCount</span></span> | <span data-ttu-id="23622-125">Int64</span><span class="sxs-lookup"><span data-stu-id="23622-125">Int64</span></span>             |
| <span data-ttu-id="23622-126">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="23622-126">assignedProducts</span></span>          | <span data-ttu-id="23622-127">字符串集合</span><span class="sxs-lookup"><span data-stu-id="23622-127">String collection</span></span> |
| <span data-ttu-id="23622-128">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="23622-128">reportPeriod</span></span>              | <span data-ttu-id="23622-129">String</span><span class="sxs-lookup"><span data-stu-id="23622-129">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="23622-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23622-130">JSON representation</span></span>

<span data-ttu-id="23622-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23622-131">The following is a JSON representation of the resource.</span></span>

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
