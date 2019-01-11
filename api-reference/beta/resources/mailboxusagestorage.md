---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: dcabfab0e8a64f2d74442f7d7464708501a59b95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840738"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="57937-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="57937-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="57937-104">属性</span><span class="sxs-lookup"><span data-stu-id="57937-104">Properties</span></span>

| <span data-ttu-id="57937-105">属性</span><span class="sxs-lookup"><span data-stu-id="57937-105">Property</span></span>           | <span data-ttu-id="57937-106">类型</span><span class="sxs-lookup"><span data-stu-id="57937-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="57937-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="57937-107">reportRefreshDate</span></span>  | <span data-ttu-id="57937-108">日期</span><span class="sxs-lookup"><span data-stu-id="57937-108">Date</span></span>   |
| <span data-ttu-id="57937-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="57937-109">storageUsedInBytes</span></span> | <span data-ttu-id="57937-110">Int64</span><span class="sxs-lookup"><span data-stu-id="57937-110">Int64</span></span>  |
| <span data-ttu-id="57937-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="57937-111">reportDate</span></span>         | <span data-ttu-id="57937-112">日期</span><span class="sxs-lookup"><span data-stu-id="57937-112">Date</span></span>   |
| <span data-ttu-id="57937-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="57937-113">reportPeriod</span></span>       | <span data-ttu-id="57937-114">String</span><span class="sxs-lookup"><span data-stu-id="57937-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57937-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57937-115">JSON representation</span></span>

<span data-ttu-id="57937-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57937-116">The following is a JSON representation of the resource.</span></span>

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
