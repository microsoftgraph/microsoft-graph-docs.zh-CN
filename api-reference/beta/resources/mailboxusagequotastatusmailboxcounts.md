---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: ac6c597cad9d28f985da97d6f55a5726ebbf491e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044372"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="c70b2-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="c70b2-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="c70b2-104">属性</span><span class="sxs-lookup"><span data-stu-id="c70b2-104">Properties</span></span>

| <span data-ttu-id="c70b2-105">属性</span><span class="sxs-lookup"><span data-stu-id="c70b2-105">Property</span></span>              | <span data-ttu-id="c70b2-106">类型</span><span class="sxs-lookup"><span data-stu-id="c70b2-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="c70b2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c70b2-107">reportRefreshDate</span></span>     | <span data-ttu-id="c70b2-108">日期</span><span class="sxs-lookup"><span data-stu-id="c70b2-108">Date</span></span>   |
| <span data-ttu-id="c70b2-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="c70b2-109">underLimit</span></span>            | <span data-ttu-id="c70b2-110">Int64</span><span class="sxs-lookup"><span data-stu-id="c70b2-110">Int64</span></span>  |
| <span data-ttu-id="c70b2-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="c70b2-111">warningIssued</span></span>         | <span data-ttu-id="c70b2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="c70b2-112">Int64</span></span>  |
| <span data-ttu-id="c70b2-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="c70b2-113">sendProhibited</span></span>        | <span data-ttu-id="c70b2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c70b2-114">Int64</span></span>  |
| <span data-ttu-id="c70b2-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="c70b2-115">sendReceiveProhibited</span></span> | <span data-ttu-id="c70b2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="c70b2-116">Int64</span></span>  |
| <span data-ttu-id="c70b2-117">不确定</span><span class="sxs-lookup"><span data-stu-id="c70b2-117">indeterminate</span></span>         | <span data-ttu-id="c70b2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="c70b2-118">Int64</span></span>  |
| <span data-ttu-id="c70b2-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="c70b2-119">reportDate</span></span>            | <span data-ttu-id="c70b2-120">日期</span><span class="sxs-lookup"><span data-stu-id="c70b2-120">Date</span></span>   |
| <span data-ttu-id="c70b2-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c70b2-121">reportPeriod</span></span>          | <span data-ttu-id="c70b2-122">String</span><span class="sxs-lookup"><span data-stu-id="c70b2-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c70b2-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c70b2-123">JSON representation</span></span>

<span data-ttu-id="c70b2-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c70b2-124">The following is a JSON representation of the resource.</span></span>

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
