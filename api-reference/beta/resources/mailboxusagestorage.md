---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8cc26c5d3cc30529857ed3273f8ee66c7373327a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043169"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="bfbce-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="bfbce-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="bfbce-104">属性</span><span class="sxs-lookup"><span data-stu-id="bfbce-104">Properties</span></span>

| <span data-ttu-id="bfbce-105">属性</span><span class="sxs-lookup"><span data-stu-id="bfbce-105">Property</span></span>           | <span data-ttu-id="bfbce-106">类型</span><span class="sxs-lookup"><span data-stu-id="bfbce-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="bfbce-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="bfbce-107">reportRefreshDate</span></span>  | <span data-ttu-id="bfbce-108">日期</span><span class="sxs-lookup"><span data-stu-id="bfbce-108">Date</span></span>   |
| <span data-ttu-id="bfbce-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="bfbce-109">storageUsedInBytes</span></span> | <span data-ttu-id="bfbce-110">Int64</span><span class="sxs-lookup"><span data-stu-id="bfbce-110">Int64</span></span>  |
| <span data-ttu-id="bfbce-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="bfbce-111">reportDate</span></span>         | <span data-ttu-id="bfbce-112">日期</span><span class="sxs-lookup"><span data-stu-id="bfbce-112">Date</span></span>   |
| <span data-ttu-id="bfbce-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="bfbce-113">reportPeriod</span></span>       | <span data-ttu-id="bfbce-114">String</span><span class="sxs-lookup"><span data-stu-id="bfbce-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfbce-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bfbce-115">JSON representation</span></span>

<span data-ttu-id="bfbce-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfbce-116">The following is a JSON representation of the resource.</span></span>

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
