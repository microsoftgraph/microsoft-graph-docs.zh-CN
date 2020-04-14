---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 636417b5ec299bb11f82c406abecdebe72ee45de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473413"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="151f4-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="151f4-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="151f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="151f4-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="151f4-105">属性</span><span class="sxs-lookup"><span data-stu-id="151f4-105">Properties</span></span>

| <span data-ttu-id="151f4-106">属性</span><span class="sxs-lookup"><span data-stu-id="151f4-106">Property</span></span>           | <span data-ttu-id="151f4-107">类型</span><span class="sxs-lookup"><span data-stu-id="151f4-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="151f4-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="151f4-108">reportRefreshDate</span></span>  | <span data-ttu-id="151f4-109">日期</span><span class="sxs-lookup"><span data-stu-id="151f4-109">Date</span></span>   |
| <span data-ttu-id="151f4-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="151f4-110">storageUsedInBytes</span></span> | <span data-ttu-id="151f4-111">Int64</span><span class="sxs-lookup"><span data-stu-id="151f4-111">Int64</span></span>  |
| <span data-ttu-id="151f4-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="151f4-112">reportDate</span></span>         | <span data-ttu-id="151f4-113">日期</span><span class="sxs-lookup"><span data-stu-id="151f4-113">Date</span></span>   |
| <span data-ttu-id="151f4-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="151f4-114">reportPeriod</span></span>       | <span data-ttu-id="151f4-115">String</span><span class="sxs-lookup"><span data-stu-id="151f4-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="151f4-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="151f4-116">JSON representation</span></span>

<span data-ttu-id="151f4-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="151f4-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
