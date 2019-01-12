---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 44b97c7b18264e01c86b34bfd8265246f80ab031
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917865"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="c7253-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7253-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c7253-104">属性</span><span class="sxs-lookup"><span data-stu-id="c7253-104">Properties</span></span>

| <span data-ttu-id="c7253-105">属性</span><span class="sxs-lookup"><span data-stu-id="c7253-105">Property</span></span>           | <span data-ttu-id="c7253-106">类型</span><span class="sxs-lookup"><span data-stu-id="c7253-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="c7253-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c7253-107">reportRefreshDate</span></span>  | <span data-ttu-id="c7253-108">日期</span><span class="sxs-lookup"><span data-stu-id="c7253-108">Date</span></span>   |
| <span data-ttu-id="c7253-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c7253-109">storageUsedInBytes</span></span> | <span data-ttu-id="c7253-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c7253-110">Int64</span></span>  |
| <span data-ttu-id="c7253-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="c7253-111">reportDate</span></span>         | <span data-ttu-id="c7253-112">日期</span><span class="sxs-lookup"><span data-stu-id="c7253-112">Date</span></span>   |
| <span data-ttu-id="c7253-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c7253-113">reportPeriod</span></span>       | <span data-ttu-id="c7253-114">String</span><span class="sxs-lookup"><span data-stu-id="c7253-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7253-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7253-115">JSON representation</span></span>

<span data-ttu-id="c7253-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7253-116">The following is a JSON representation of the resource.</span></span>

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
