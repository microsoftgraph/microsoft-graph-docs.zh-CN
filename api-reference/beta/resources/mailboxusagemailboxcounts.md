---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e9da6a72c3c2d79323041e683702a7af2e4699c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463269"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="630a5-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="630a5-103">mailboxUsageMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="630a5-104">属性</span><span class="sxs-lookup"><span data-stu-id="630a5-104">Properties</span></span>

| <span data-ttu-id="630a5-105">属性</span><span class="sxs-lookup"><span data-stu-id="630a5-105">Property</span></span>          | <span data-ttu-id="630a5-106">类型</span><span class="sxs-lookup"><span data-stu-id="630a5-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="630a5-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="630a5-107">reportRefreshDate</span></span> | <span data-ttu-id="630a5-108">Date</span><span class="sxs-lookup"><span data-stu-id="630a5-108">Date</span></span>   |
| <span data-ttu-id="630a5-109">total</span><span class="sxs-lookup"><span data-stu-id="630a5-109">total</span></span>             | <span data-ttu-id="630a5-110">Int64</span><span class="sxs-lookup"><span data-stu-id="630a5-110">Int64</span></span>  |
| <span data-ttu-id="630a5-111">工作</span><span class="sxs-lookup"><span data-stu-id="630a5-111">active</span></span>            | <span data-ttu-id="630a5-112">Int64</span><span class="sxs-lookup"><span data-stu-id="630a5-112">Int64</span></span>  |
| <span data-ttu-id="630a5-113">reportDate</span><span class="sxs-lookup"><span data-stu-id="630a5-113">reportDate</span></span>        | <span data-ttu-id="630a5-114">Date</span><span class="sxs-lookup"><span data-stu-id="630a5-114">Date</span></span>   |
| <span data-ttu-id="630a5-115">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="630a5-115">reportPeriod</span></span>      | <span data-ttu-id="630a5-116">字符串</span><span class="sxs-lookup"><span data-stu-id="630a5-116">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="630a5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="630a5-117">JSON representation</span></span>

<span data-ttu-id="630a5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="630a5-118">The following is a JSON representation of the resource.</span></span>

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
