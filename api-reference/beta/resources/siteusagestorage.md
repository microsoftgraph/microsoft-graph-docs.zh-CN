---
title: siteUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 1f656feacdbba3418049bd9f3072270aa04af798
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879924"
---
# <a name="siteusagestorage-resource-type"></a><span data-ttu-id="d4875-103">siteUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4875-103">siteUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d4875-104">属性</span><span class="sxs-lookup"><span data-stu-id="d4875-104">Properties</span></span>

| <span data-ttu-id="d4875-105">属性</span><span class="sxs-lookup"><span data-stu-id="d4875-105">Property</span></span>           | <span data-ttu-id="d4875-106">类型</span><span class="sxs-lookup"><span data-stu-id="d4875-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="d4875-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d4875-107">reportRefreshDate</span></span>  | <span data-ttu-id="d4875-108">日期</span><span class="sxs-lookup"><span data-stu-id="d4875-108">Date</span></span>   |
| <span data-ttu-id="d4875-109">键入一个文件夹</span><span class="sxs-lookup"><span data-stu-id="d4875-109">siteType</span></span>           | <span data-ttu-id="d4875-110">字符串</span><span class="sxs-lookup"><span data-stu-id="d4875-110">String</span></span> |
| <span data-ttu-id="d4875-111">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d4875-111">storageUsedInBytes</span></span> | <span data-ttu-id="d4875-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d4875-112">Int64</span></span>  |
| <span data-ttu-id="d4875-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="d4875-113">reportDate</span></span>         | <span data-ttu-id="d4875-114">日期</span><span class="sxs-lookup"><span data-stu-id="d4875-114">Date</span></span>   |
| <span data-ttu-id="d4875-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d4875-115">reportPeriod</span></span>       | <span data-ttu-id="d4875-116">String</span><span class="sxs-lookup"><span data-stu-id="d4875-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d4875-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4875-117">JSON representation</span></span>

<span data-ttu-id="d4875-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4875-118">The following is a JSON representation of the resource.</span></span>

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
