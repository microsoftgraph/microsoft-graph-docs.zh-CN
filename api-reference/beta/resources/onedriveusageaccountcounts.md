---
title: oneDriveUsageAccountCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: JeremyKelley
ms.openlocfilehash: 770968141305275f33609db3deca8bb77f5d51cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039312"
---
# <a name="onedriveusageaccountcounts-resource-type"></a><span data-ttu-id="2a56b-103">oneDriveUsageAccountCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a56b-103">oneDriveUsageAccountCounts resource type</span></span>

<span data-ttu-id="2a56b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a56b-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2a56b-105">属性</span><span class="sxs-lookup"><span data-stu-id="2a56b-105">Properties</span></span>

| <span data-ttu-id="2a56b-106">属性</span><span class="sxs-lookup"><span data-stu-id="2a56b-106">Property</span></span>          | <span data-ttu-id="2a56b-107">类型</span><span class="sxs-lookup"><span data-stu-id="2a56b-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="2a56b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2a56b-108">reportRefreshDate</span></span> | <span data-ttu-id="2a56b-109">日期</span><span class="sxs-lookup"><span data-stu-id="2a56b-109">Date</span></span>   |
| <span data-ttu-id="2a56b-110">siteType</span><span class="sxs-lookup"><span data-stu-id="2a56b-110">siteType</span></span>          | <span data-ttu-id="2a56b-111">String</span><span class="sxs-lookup"><span data-stu-id="2a56b-111">String</span></span> |
| <span data-ttu-id="2a56b-112">total</span><span class="sxs-lookup"><span data-stu-id="2a56b-112">total</span></span>             | <span data-ttu-id="2a56b-113">Int64</span><span class="sxs-lookup"><span data-stu-id="2a56b-113">Int64</span></span>  |
| <span data-ttu-id="2a56b-114">工作</span><span class="sxs-lookup"><span data-stu-id="2a56b-114">active</span></span>            | <span data-ttu-id="2a56b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2a56b-115">Int64</span></span>  |
| <span data-ttu-id="2a56b-116">reportDate</span><span class="sxs-lookup"><span data-stu-id="2a56b-116">reportDate</span></span>        | <span data-ttu-id="2a56b-117">日期</span><span class="sxs-lookup"><span data-stu-id="2a56b-117">Date</span></span>   |
| <span data-ttu-id="2a56b-118">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2a56b-118">reportPeriod</span></span>      | <span data-ttu-id="2a56b-119">String</span><span class="sxs-lookup"><span data-stu-id="2a56b-119">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2a56b-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a56b-120">JSON representation</span></span>

<span data-ttu-id="2a56b-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a56b-121">The following is a JSON representation of the resource.</span></span>

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


