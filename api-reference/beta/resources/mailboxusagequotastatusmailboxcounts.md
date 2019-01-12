---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 45e4754fef0dd3a2f7a669e3b3b96692d117c8f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921232"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="e7ea2-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7ea2-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e7ea2-104">属性</span><span class="sxs-lookup"><span data-stu-id="e7ea2-104">Properties</span></span>

| <span data-ttu-id="e7ea2-105">属性</span><span class="sxs-lookup"><span data-stu-id="e7ea2-105">Property</span></span>              | <span data-ttu-id="e7ea2-106">类型</span><span class="sxs-lookup"><span data-stu-id="e7ea2-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="e7ea2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e7ea2-107">reportRefreshDate</span></span>     | <span data-ttu-id="e7ea2-108">日期</span><span class="sxs-lookup"><span data-stu-id="e7ea2-108">Date</span></span>   |
| <span data-ttu-id="e7ea2-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="e7ea2-109">underLimit</span></span>            | <span data-ttu-id="e7ea2-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e7ea2-110">Int64</span></span>  |
| <span data-ttu-id="e7ea2-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="e7ea2-111">warningIssued</span></span>         | <span data-ttu-id="e7ea2-112">Int64</span><span class="sxs-lookup"><span data-stu-id="e7ea2-112">Int64</span></span>  |
| <span data-ttu-id="e7ea2-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="e7ea2-113">sendProhibited</span></span>        | <span data-ttu-id="e7ea2-114">Int64</span><span class="sxs-lookup"><span data-stu-id="e7ea2-114">Int64</span></span>  |
| <span data-ttu-id="e7ea2-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="e7ea2-115">sendReceiveProhibited</span></span> | <span data-ttu-id="e7ea2-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e7ea2-116">Int64</span></span>  |
| <span data-ttu-id="e7ea2-117">不确定</span><span class="sxs-lookup"><span data-stu-id="e7ea2-117">indeterminate</span></span>         | <span data-ttu-id="e7ea2-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e7ea2-118">Int64</span></span>  |
| <span data-ttu-id="e7ea2-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="e7ea2-119">reportDate</span></span>            | <span data-ttu-id="e7ea2-120">日期</span><span class="sxs-lookup"><span data-stu-id="e7ea2-120">Date</span></span>   |
| <span data-ttu-id="e7ea2-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e7ea2-121">reportPeriod</span></span>          | <span data-ttu-id="e7ea2-122">String</span><span class="sxs-lookup"><span data-stu-id="e7ea2-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e7ea2-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7ea2-123">JSON representation</span></span>

<span data-ttu-id="e7ea2-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7ea2-124">The following is a JSON representation of the resource.</span></span>

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
