---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 1fdfa6cb2690d6dbacf5e534792061b6e64025d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042718"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="455f9-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="455f9-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="455f9-104">属性</span><span class="sxs-lookup"><span data-stu-id="455f9-104">Properties</span></span>

| <span data-ttu-id="455f9-105">属性</span><span class="sxs-lookup"><span data-stu-id="455f9-105">Property</span></span>           | <span data-ttu-id="455f9-106">类型</span><span class="sxs-lookup"><span data-stu-id="455f9-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="455f9-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="455f9-107">reportRefreshDate</span></span>  | <span data-ttu-id="455f9-108">日期</span><span class="sxs-lookup"><span data-stu-id="455f9-108">Date</span></span>   |
| <span data-ttu-id="455f9-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="455f9-109">siteType</span></span>           | <span data-ttu-id="455f9-110">字符串</span><span class="sxs-lookup"><span data-stu-id="455f9-110">String</span></span> |
| <span data-ttu-id="455f9-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="455f9-111">storageUsedInBytes</span></span> | <span data-ttu-id="455f9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="455f9-112">Int64</span></span>  |
| <span data-ttu-id="455f9-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="455f9-113">reportDate</span></span>         | <span data-ttu-id="455f9-114">日期</span><span class="sxs-lookup"><span data-stu-id="455f9-114">Date</span></span>   |
| <span data-ttu-id="455f9-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="455f9-115">reportPeriod</span></span>       | <span data-ttu-id="455f9-116">String</span><span class="sxs-lookup"><span data-stu-id="455f9-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="455f9-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="455f9-117">JSON representation</span></span>

<span data-ttu-id="455f9-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="455f9-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteUsageStorage"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "siteType": "String", 
  "storageUsedInBytes": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
