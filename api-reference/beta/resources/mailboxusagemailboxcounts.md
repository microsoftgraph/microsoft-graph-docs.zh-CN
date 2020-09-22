---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e8282422f9724cbffff8f3e9573f0a7cb0a94920
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971816"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="0ba72-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="0ba72-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="0ba72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ba72-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0ba72-105">属性</span><span class="sxs-lookup"><span data-stu-id="0ba72-105">Properties</span></span>

| <span data-ttu-id="0ba72-106">属性</span><span class="sxs-lookup"><span data-stu-id="0ba72-106">Property</span></span>          | <span data-ttu-id="0ba72-107">类型</span><span class="sxs-lookup"><span data-stu-id="0ba72-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="0ba72-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0ba72-108">reportRefreshDate</span></span> | <span data-ttu-id="0ba72-109">日期</span><span class="sxs-lookup"><span data-stu-id="0ba72-109">Date</span></span>   |
| <span data-ttu-id="0ba72-110">total</span><span class="sxs-lookup"><span data-stu-id="0ba72-110">total</span></span>             | <span data-ttu-id="0ba72-111">Int64</span><span class="sxs-lookup"><span data-stu-id="0ba72-111">Int64</span></span>  |
| <span data-ttu-id="0ba72-112">工作</span><span class="sxs-lookup"><span data-stu-id="0ba72-112">active</span></span>            | <span data-ttu-id="0ba72-113">Int64</span><span class="sxs-lookup"><span data-stu-id="0ba72-113">Int64</span></span>  |
| <span data-ttu-id="0ba72-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="0ba72-114">reportDate</span></span>        | <span data-ttu-id="0ba72-115">日期</span><span class="sxs-lookup"><span data-stu-id="0ba72-115">Date</span></span>   |
| <span data-ttu-id="0ba72-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0ba72-116">reportPeriod</span></span>      | <span data-ttu-id="0ba72-117">String</span><span class="sxs-lookup"><span data-stu-id="0ba72-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0ba72-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0ba72-118">JSON representation</span></span>

<span data-ttu-id="0ba72-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ba72-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "total": 1024, 
  "active": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


