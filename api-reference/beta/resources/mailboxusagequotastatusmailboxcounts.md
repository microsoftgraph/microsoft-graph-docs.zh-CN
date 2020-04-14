---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1ebbfe0f134848d78e9c42a159c1c56bdbd21b39
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473423"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="b1acd-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1acd-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="b1acd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1acd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b1acd-105">属性</span><span class="sxs-lookup"><span data-stu-id="b1acd-105">Properties</span></span>

| <span data-ttu-id="b1acd-106">属性</span><span class="sxs-lookup"><span data-stu-id="b1acd-106">Property</span></span>              | <span data-ttu-id="b1acd-107">类型</span><span class="sxs-lookup"><span data-stu-id="b1acd-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="b1acd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b1acd-108">reportRefreshDate</span></span>     | <span data-ttu-id="b1acd-109">日期</span><span class="sxs-lookup"><span data-stu-id="b1acd-109">Date</span></span>   |
| <span data-ttu-id="b1acd-110">underLimit</span><span class="sxs-lookup"><span data-stu-id="b1acd-110">underLimit</span></span>            | <span data-ttu-id="b1acd-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b1acd-111">Int64</span></span>  |
| <span data-ttu-id="b1acd-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="b1acd-112">warningIssued</span></span>         | <span data-ttu-id="b1acd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b1acd-113">Int64</span></span>  |
| <span data-ttu-id="b1acd-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="b1acd-114">sendProhibited</span></span>        | <span data-ttu-id="b1acd-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b1acd-115">Int64</span></span>  |
| <span data-ttu-id="b1acd-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="b1acd-116">sendReceiveProhibited</span></span> | <span data-ttu-id="b1acd-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b1acd-117">Int64</span></span>  |
| <span data-ttu-id="b1acd-118">尚</span><span class="sxs-lookup"><span data-stu-id="b1acd-118">indeterminate</span></span>         | <span data-ttu-id="b1acd-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b1acd-119">Int64</span></span>  |
| <span data-ttu-id="b1acd-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="b1acd-120">reportDate</span></span>            | <span data-ttu-id="b1acd-121">日期</span><span class="sxs-lookup"><span data-stu-id="b1acd-121">Date</span></span>   |
| <span data-ttu-id="b1acd-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b1acd-122">reportPeriod</span></span>          | <span data-ttu-id="b1acd-123">String</span><span class="sxs-lookup"><span data-stu-id="b1acd-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1acd-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1acd-124">JSON representation</span></span>

<span data-ttu-id="b1acd-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1acd-125">The following is a JSON representation of the resource.</span></span>

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
