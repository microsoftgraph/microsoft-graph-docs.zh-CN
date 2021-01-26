---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 10ce05121ec900f5475a082191f4192974f980b4
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983543"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="a22ef-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a22ef-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

<span data-ttu-id="a22ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a22ef-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a22ef-105">属性</span><span class="sxs-lookup"><span data-stu-id="a22ef-105">Properties</span></span>

| <span data-ttu-id="a22ef-106">属性</span><span class="sxs-lookup"><span data-stu-id="a22ef-106">Property</span></span>              | <span data-ttu-id="a22ef-107">类型</span><span class="sxs-lookup"><span data-stu-id="a22ef-107">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="a22ef-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a22ef-108">reportRefreshDate</span></span>     | <span data-ttu-id="a22ef-109">日期</span><span class="sxs-lookup"><span data-stu-id="a22ef-109">Date</span></span>   |
| <span data-ttu-id="a22ef-110">underLimit</span><span class="sxs-lookup"><span data-stu-id="a22ef-110">underLimit</span></span>            | <span data-ttu-id="a22ef-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a22ef-111">Int64</span></span>  |
| <span data-ttu-id="a22ef-112">warningIssued</span><span class="sxs-lookup"><span data-stu-id="a22ef-112">warningIssued</span></span>         | <span data-ttu-id="a22ef-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a22ef-113">Int64</span></span>  |
| <span data-ttu-id="a22ef-114">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="a22ef-114">sendProhibited</span></span>        | <span data-ttu-id="a22ef-115">Int64</span><span class="sxs-lookup"><span data-stu-id="a22ef-115">Int64</span></span>  |
| <span data-ttu-id="a22ef-116">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="a22ef-116">sendReceiveProhibited</span></span> | <span data-ttu-id="a22ef-117">Int64</span><span class="sxs-lookup"><span data-stu-id="a22ef-117">Int64</span></span>  |
| <span data-ttu-id="a22ef-118">不确定</span><span class="sxs-lookup"><span data-stu-id="a22ef-118">indeterminate</span></span>         | <span data-ttu-id="a22ef-119">Int64</span><span class="sxs-lookup"><span data-stu-id="a22ef-119">Int64</span></span>  |
| <span data-ttu-id="a22ef-120">reportDate</span><span class="sxs-lookup"><span data-stu-id="a22ef-120">reportDate</span></span>            | <span data-ttu-id="a22ef-121">日期</span><span class="sxs-lookup"><span data-stu-id="a22ef-121">Date</span></span>   |
| <span data-ttu-id="a22ef-122">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a22ef-122">reportPeriod</span></span>          | <span data-ttu-id="a22ef-123">String</span><span class="sxs-lookup"><span data-stu-id="a22ef-123">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a22ef-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a22ef-124">JSON representation</span></span>

<span data-ttu-id="a22ef-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a22ef-125">The following is a JSON representation of the resource.</span></span>

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


