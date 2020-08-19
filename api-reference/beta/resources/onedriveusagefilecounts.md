---
title: oneDriveUsageFileCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 0beb20ee592f5131ebefe3a3e547131b3903d762
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812076"
---
# <a name="onedriveusagefilecounts-resource-type"></a><span data-ttu-id="c4248-103">oneDriveUsageFileCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4248-103">oneDriveUsageFileCounts resource type</span></span>

<span data-ttu-id="c4248-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4248-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c4248-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4248-105">Properties</span></span>

| <span data-ttu-id="c4248-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4248-106">Property</span></span>          | <span data-ttu-id="c4248-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4248-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="c4248-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c4248-108">reportRefreshDate</span></span> | <span data-ttu-id="c4248-109">日期</span><span class="sxs-lookup"><span data-stu-id="c4248-109">Date</span></span>   |
| <span data-ttu-id="c4248-110">siteType</span><span class="sxs-lookup"><span data-stu-id="c4248-110">siteType</span></span>          | <span data-ttu-id="c4248-111">String</span><span class="sxs-lookup"><span data-stu-id="c4248-111">String</span></span> |
| <span data-ttu-id="c4248-112">total</span><span class="sxs-lookup"><span data-stu-id="c4248-112">total</span></span>             | <span data-ttu-id="c4248-113">Int64</span><span class="sxs-lookup"><span data-stu-id="c4248-113">Int64</span></span>  |
| <span data-ttu-id="c4248-114">工作</span><span class="sxs-lookup"><span data-stu-id="c4248-114">active</span></span>            | <span data-ttu-id="c4248-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c4248-115">Int64</span></span>  |
| <span data-ttu-id="c4248-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="c4248-116">reportDate</span></span>        | <span data-ttu-id="c4248-117">日期</span><span class="sxs-lookup"><span data-stu-id="c4248-117">Date</span></span>   |
| <span data-ttu-id="c4248-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c4248-118">reportPeriod</span></span>      | <span data-ttu-id="c4248-119">String</span><span class="sxs-lookup"><span data-stu-id="c4248-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c4248-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4248-120">JSON representation</span></span>

<span data-ttu-id="c4248-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4248-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```json
{
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```
