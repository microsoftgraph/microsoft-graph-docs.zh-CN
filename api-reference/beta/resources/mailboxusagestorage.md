---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6f4ee4b29c82102db96cd4d71718f7da449776b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009837"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="494c0-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="494c0-103">mailboxUsageStorage resource type</span></span>

## <a name="properties"></a><span data-ttu-id="494c0-104">属性</span><span class="sxs-lookup"><span data-stu-id="494c0-104">Properties</span></span>

| <span data-ttu-id="494c0-105">属性</span><span class="sxs-lookup"><span data-stu-id="494c0-105">Property</span></span>           | <span data-ttu-id="494c0-106">类型</span><span class="sxs-lookup"><span data-stu-id="494c0-106">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="494c0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="494c0-107">reportRefreshDate</span></span>  | <span data-ttu-id="494c0-108">日期</span><span class="sxs-lookup"><span data-stu-id="494c0-108">Date</span></span>   |
| <span data-ttu-id="494c0-109">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="494c0-109">storageUsedInBytes</span></span> | <span data-ttu-id="494c0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="494c0-110">Int64</span></span>  |
| <span data-ttu-id="494c0-111">reportDate</span><span class="sxs-lookup"><span data-stu-id="494c0-111">reportDate</span></span>         | <span data-ttu-id="494c0-112">日期</span><span class="sxs-lookup"><span data-stu-id="494c0-112">Date</span></span>   |
| <span data-ttu-id="494c0-113">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="494c0-113">reportPeriod</span></span>       | <span data-ttu-id="494c0-114">String</span><span class="sxs-lookup"><span data-stu-id="494c0-114">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="494c0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="494c0-115">JSON representation</span></span>

<span data-ttu-id="494c0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="494c0-116">The following is a JSON representation of the resource.</span></span>

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
