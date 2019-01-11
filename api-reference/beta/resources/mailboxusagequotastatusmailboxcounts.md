---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: b87bb1ce91626f9151d294e2243bba72ba72346b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835218"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="91207-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="91207-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="91207-104">属性</span><span class="sxs-lookup"><span data-stu-id="91207-104">Properties</span></span>

| <span data-ttu-id="91207-105">属性</span><span class="sxs-lookup"><span data-stu-id="91207-105">Property</span></span>              | <span data-ttu-id="91207-106">类型</span><span class="sxs-lookup"><span data-stu-id="91207-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="91207-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="91207-107">reportRefreshDate</span></span>     | <span data-ttu-id="91207-108">日期</span><span class="sxs-lookup"><span data-stu-id="91207-108">Date</span></span>   |
| <span data-ttu-id="91207-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="91207-109">underLimit</span></span>            | <span data-ttu-id="91207-110">Int64</span><span class="sxs-lookup"><span data-stu-id="91207-110">Int64</span></span>  |
| <span data-ttu-id="91207-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="91207-111">warningIssued</span></span>         | <span data-ttu-id="91207-112">Int64</span><span class="sxs-lookup"><span data-stu-id="91207-112">Int64</span></span>  |
| <span data-ttu-id="91207-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="91207-113">sendProhibited</span></span>        | <span data-ttu-id="91207-114">Int64</span><span class="sxs-lookup"><span data-stu-id="91207-114">Int64</span></span>  |
| <span data-ttu-id="91207-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="91207-115">sendReceiveProhibited</span></span> | <span data-ttu-id="91207-116">Int64</span><span class="sxs-lookup"><span data-stu-id="91207-116">Int64</span></span>  |
| <span data-ttu-id="91207-117">不确定</span><span class="sxs-lookup"><span data-stu-id="91207-117">indeterminate</span></span>         | <span data-ttu-id="91207-118">Int64</span><span class="sxs-lookup"><span data-stu-id="91207-118">Int64</span></span>  |
| <span data-ttu-id="91207-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="91207-119">reportDate</span></span>            | <span data-ttu-id="91207-120">日期</span><span class="sxs-lookup"><span data-stu-id="91207-120">Date</span></span>   |
| <span data-ttu-id="91207-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="91207-121">reportPeriod</span></span>          | <span data-ttu-id="91207-122">String</span><span class="sxs-lookup"><span data-stu-id="91207-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="91207-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91207-123">JSON representation</span></span>

<span data-ttu-id="91207-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91207-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "underLimit": 1024, 
  "warningIssued": 1024, 
  "sendProhibited": 1024, 
  "sendReceiveProhibited": 1024, 
  "indeterminate": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
