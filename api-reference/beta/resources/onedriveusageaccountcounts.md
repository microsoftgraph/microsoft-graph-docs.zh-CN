---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 8ab079eb15fd2dfe2d66a07d5734b6aa9430055e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812111"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="09cff-103">oneDriveUsageAccountCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="09cff-103">oneDriveUsageAccountCounts resource type</span></span>

<span data-ttu-id="09cff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09cff-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="09cff-105">属性</span><span class="sxs-lookup"><span data-stu-id="09cff-105">Properties</span></span>

| <span data-ttu-id="09cff-106">属性</span><span class="sxs-lookup"><span data-stu-id="09cff-106">Property</span></span>          | <span data-ttu-id="09cff-107">类型</span><span class="sxs-lookup"><span data-stu-id="09cff-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="09cff-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="09cff-108">reportRefreshDate</span></span> | <span data-ttu-id="09cff-109">日期</span><span class="sxs-lookup"><span data-stu-id="09cff-109">Date</span></span>   |
| <span data-ttu-id="09cff-110">siteType</span><span class="sxs-lookup"><span data-stu-id="09cff-110">siteType</span></span>          | <span data-ttu-id="09cff-111">String</span><span class="sxs-lookup"><span data-stu-id="09cff-111">String</span></span> |
| <span data-ttu-id="09cff-112">total</span><span class="sxs-lookup"><span data-stu-id="09cff-112">total</span></span>             | <span data-ttu-id="09cff-113">Int64</span><span class="sxs-lookup"><span data-stu-id="09cff-113">Int64</span></span>  |
| <span data-ttu-id="09cff-114">工作</span><span class="sxs-lookup"><span data-stu-id="09cff-114">active</span></span>            | <span data-ttu-id="09cff-115">Int64</span><span class="sxs-lookup"><span data-stu-id="09cff-115">Int64</span></span>  |
| <span data-ttu-id="09cff-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="09cff-116">reportDate</span></span>        | <span data-ttu-id="09cff-117">日期</span><span class="sxs-lookup"><span data-stu-id="09cff-117">Date</span></span>   |
| <span data-ttu-id="09cff-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="09cff-118">reportPeriod</span></span>      | <span data-ttu-id="09cff-119">String</span><span class="sxs-lookup"><span data-stu-id="09cff-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="09cff-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09cff-120">JSON representation</span></span>

<span data-ttu-id="09cff-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09cff-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
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
