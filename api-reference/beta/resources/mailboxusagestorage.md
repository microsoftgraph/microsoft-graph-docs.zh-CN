---
title: mailboxUsageStorage 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 080b1e5eafb23e40df1307fc6ab3e9a4ef9c87f0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075530"
---
# <a name="mailboxusagestorage-resource-type"></a><span data-ttu-id="69ac1-103">mailboxUsageStorage 资源类型</span><span class="sxs-lookup"><span data-stu-id="69ac1-103">mailboxUsageStorage resource type</span></span>

<span data-ttu-id="69ac1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69ac1-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="69ac1-105">属性</span><span class="sxs-lookup"><span data-stu-id="69ac1-105">Properties</span></span>

| <span data-ttu-id="69ac1-106">属性</span><span class="sxs-lookup"><span data-stu-id="69ac1-106">Property</span></span>           | <span data-ttu-id="69ac1-107">类型</span><span class="sxs-lookup"><span data-stu-id="69ac1-107">Type</span></span>   |
| :----------------- | :----- |
| <span data-ttu-id="69ac1-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="69ac1-108">reportRefreshDate</span></span>  | <span data-ttu-id="69ac1-109">日期</span><span class="sxs-lookup"><span data-stu-id="69ac1-109">Date</span></span>   |
| <span data-ttu-id="69ac1-110">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="69ac1-110">storageUsedInBytes</span></span> | <span data-ttu-id="69ac1-111">Int64</span><span class="sxs-lookup"><span data-stu-id="69ac1-111">Int64</span></span>  |
| <span data-ttu-id="69ac1-112">reportDate</span><span class="sxs-lookup"><span data-stu-id="69ac1-112">reportDate</span></span>         | <span data-ttu-id="69ac1-113">日期</span><span class="sxs-lookup"><span data-stu-id="69ac1-113">Date</span></span>   |
| <span data-ttu-id="69ac1-114">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="69ac1-114">reportPeriod</span></span>       | <span data-ttu-id="69ac1-115">String</span><span class="sxs-lookup"><span data-stu-id="69ac1-115">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="69ac1-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69ac1-116">JSON representation</span></span>

<span data-ttu-id="69ac1-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69ac1-117">The following is a JSON representation of the resource.</span></span>

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


