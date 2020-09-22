---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e09b9d27da4a85dd89f6a09440d56532045573b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029174"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="ba2a1-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba2a1-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="ba2a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2a1-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="ba2a1-105">属性</span><span class="sxs-lookup"><span data-stu-id="ba2a1-105">Properties</span></span>

| <span data-ttu-id="ba2a1-106">属性</span><span class="sxs-lookup"><span data-stu-id="ba2a1-106">Property</span></span>              | <span data-ttu-id="ba2a1-107">类型</span><span class="sxs-lookup"><span data-stu-id="ba2a1-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="ba2a1-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ba2a1-108">reportRefreshDate</span></span>     | <span data-ttu-id="ba2a1-109">日期</span><span class="sxs-lookup"><span data-stu-id="ba2a1-109">Date</span></span>   |
| <span data-ttu-id="ba2a1-110">underLimit</span><span class="sxs-lookup"><span data-stu-id="ba2a1-110">underLimit</span></span>            | <span data-ttu-id="ba2a1-111">Int64</span><span class="sxs-lookup"><span data-stu-id="ba2a1-111">Int64</span></span>  |
| <span data-ttu-id="ba2a1-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="ba2a1-112">warningIssued</span></span>         | <span data-ttu-id="ba2a1-113">Int64</span><span class="sxs-lookup"><span data-stu-id="ba2a1-113">Int64</span></span>  |
| <span data-ttu-id="ba2a1-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="ba2a1-114">sendProhibited</span></span>        | <span data-ttu-id="ba2a1-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ba2a1-115">Int64</span></span>  |
| <span data-ttu-id="ba2a1-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="ba2a1-116">sendReceiveProhibited</span></span> | <span data-ttu-id="ba2a1-117">Int64</span><span class="sxs-lookup"><span data-stu-id="ba2a1-117">Int64</span></span>  |
| <span data-ttu-id="ba2a1-118">尚</span><span class="sxs-lookup"><span data-stu-id="ba2a1-118">indeterminate</span></span>         | <span data-ttu-id="ba2a1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ba2a1-119">Int64</span></span>  |
| <span data-ttu-id="ba2a1-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="ba2a1-120">reportDate</span></span>            | <span data-ttu-id="ba2a1-121">日期</span><span class="sxs-lookup"><span data-stu-id="ba2a1-121">Date</span></span>   |
| <span data-ttu-id="ba2a1-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ba2a1-122">reportPeriod</span></span>          | <span data-ttu-id="ba2a1-123">String</span><span class="sxs-lookup"><span data-stu-id="ba2a1-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba2a1-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba2a1-124">JSON representation</span></span>

<span data-ttu-id="ba2a1-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba2a1-125">The following is a JSON representation of the resource.</span></span>

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


