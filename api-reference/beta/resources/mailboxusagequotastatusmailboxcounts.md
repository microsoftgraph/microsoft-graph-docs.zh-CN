---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: ce215e0eae3a13aa0c2d27f54338efc57c0c5486
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522839"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="b9c61-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9c61-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="b9c61-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b9c61-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b9c61-105">属性</span><span class="sxs-lookup"><span data-stu-id="b9c61-105">Properties</span></span>

| <span data-ttu-id="b9c61-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9c61-106">Property</span></span>              | <span data-ttu-id="b9c61-107">类型</span><span class="sxs-lookup"><span data-stu-id="b9c61-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="b9c61-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b9c61-108">reportRefreshDate</span></span>     | <span data-ttu-id="b9c61-109">日期</span><span class="sxs-lookup"><span data-stu-id="b9c61-109">Date</span></span>   |
| <span data-ttu-id="b9c61-110">underLimit</span><span class="sxs-lookup"><span data-stu-id="b9c61-110">underLimit</span></span>            | <span data-ttu-id="b9c61-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b9c61-111">Int64</span></span>  |
| <span data-ttu-id="b9c61-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="b9c61-112">warningIssued</span></span>         | <span data-ttu-id="b9c61-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b9c61-113">Int64</span></span>  |
| <span data-ttu-id="b9c61-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="b9c61-114">sendProhibited</span></span>        | <span data-ttu-id="b9c61-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b9c61-115">Int64</span></span>  |
| <span data-ttu-id="b9c61-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="b9c61-116">sendReceiveProhibited</span></span> | <span data-ttu-id="b9c61-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b9c61-117">Int64</span></span>  |
| <span data-ttu-id="b9c61-118">尚</span><span class="sxs-lookup"><span data-stu-id="b9c61-118">indeterminate</span></span>         | <span data-ttu-id="b9c61-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b9c61-119">Int64</span></span>  |
| <span data-ttu-id="b9c61-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="b9c61-120">reportDate</span></span>            | <span data-ttu-id="b9c61-121">日期</span><span class="sxs-lookup"><span data-stu-id="b9c61-121">Date</span></span>   |
| <span data-ttu-id="b9c61-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b9c61-122">reportPeriod</span></span>          | <span data-ttu-id="b9c61-123">String</span><span class="sxs-lookup"><span data-stu-id="b9c61-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9c61-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9c61-124">JSON representation</span></span>

<span data-ttu-id="b9c61-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9c61-125">The following is a JSON representation of the resource.</span></span>

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
