---
title: emailAppUsageVersionsUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 02869749e3991d53cfd949d4e0d8c78727a91d06
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413273"
---
# <a name="emailappusageversionsusercounts-resource-type"></a><span data-ttu-id="319be-103">emailAppUsageVersionsUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="319be-103">emailAppUsageVersionsUserCounts resource type</span></span>

<span data-ttu-id="319be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="319be-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="319be-105">属性</span><span class="sxs-lookup"><span data-stu-id="319be-105">Properties</span></span>

| <span data-ttu-id="319be-106">属性</span><span class="sxs-lookup"><span data-stu-id="319be-106">Property</span></span>          | <span data-ttu-id="319be-107">类型</span><span class="sxs-lookup"><span data-stu-id="319be-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="319be-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="319be-108">reportRefreshDate</span></span> | <span data-ttu-id="319be-109">日期</span><span class="sxs-lookup"><span data-stu-id="319be-109">Date</span></span>   |
| <span data-ttu-id="319be-110">outlook2016</span><span class="sxs-lookup"><span data-stu-id="319be-110">outlook2016</span></span>       | <span data-ttu-id="319be-111">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-111">Int64</span></span>  |
| <span data-ttu-id="319be-112">outlook2013</span><span class="sxs-lookup"><span data-stu-id="319be-112">outlook2013</span></span>       | <span data-ttu-id="319be-113">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-113">Int64</span></span>  |
| <span data-ttu-id="319be-114">outlook2010</span><span class="sxs-lookup"><span data-stu-id="319be-114">outlook2010</span></span>       | <span data-ttu-id="319be-115">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-115">Int64</span></span>  |
| <span data-ttu-id="319be-116">outlook2007</span><span class="sxs-lookup"><span data-stu-id="319be-116">outlook2007</span></span>       | <span data-ttu-id="319be-117">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-117">Int64</span></span>  |
| <span data-ttu-id="319be-118">流程</span><span class="sxs-lookup"><span data-stu-id="319be-118">undetermined</span></span>      | <span data-ttu-id="319be-119">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-119">Int64</span></span>  |
| <span data-ttu-id="319be-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="319be-120">reportPeriod</span></span>      | <span data-ttu-id="319be-121">String</span><span class="sxs-lookup"><span data-stu-id="319be-121">String</span></span> |
| <span data-ttu-id="319be-122">outlookM365</span><span class="sxs-lookup"><span data-stu-id="319be-122">outlookM365</span></span>       | <span data-ttu-id="319be-123">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-123">Int64</span></span>  |
| <span data-ttu-id="319be-124">outlook2019</span><span class="sxs-lookup"><span data-stu-id="319be-124">outlook2019</span></span>       | <span data-ttu-id="319be-125">Int64</span><span class="sxs-lookup"><span data-stu-id="319be-125">Int64</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="319be-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="319be-126">JSON representation</span></span>

<span data-ttu-id="319be-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="319be-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailAppUsageVersionsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "outlook2016": 1024, 
  "outlook2013": 1024, 
  "outlook2010": 1024, 
  "outlook2007": 1024, 
  "undetermined": 1024, 
  "reportPeriod": "String",
  "outlookM365": 1024,
  "outlook2019": 1024
}
```
