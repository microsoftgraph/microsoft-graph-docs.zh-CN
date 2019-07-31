---
title: mailboxUsageQuotaStatusMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e8fafe9a3cdce4519cf5755337b016fa587cd06
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966900"
---
# <a name="mailboxusagequotastatusmailboxcounts-resource-type"></a><span data-ttu-id="d810c-103">mailboxUsageQuotaStatusMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="d810c-103">mailboxUsageQuotaStatusMailboxCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d810c-104">属性</span><span class="sxs-lookup"><span data-stu-id="d810c-104">Properties</span></span>

| <span data-ttu-id="d810c-105">属性</span><span class="sxs-lookup"><span data-stu-id="d810c-105">Property</span></span>              | <span data-ttu-id="d810c-106">类型</span><span class="sxs-lookup"><span data-stu-id="d810c-106">Type</span></span>   |
| :-------------------- | :----- |
| <span data-ttu-id="d810c-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d810c-107">reportRefreshDate</span></span>     | <span data-ttu-id="d810c-108">日期</span><span class="sxs-lookup"><span data-stu-id="d810c-108">Date</span></span>   |
| <span data-ttu-id="d810c-109">underLimit</span><span class="sxs-lookup"><span data-stu-id="d810c-109">underLimit</span></span>            | <span data-ttu-id="d810c-110">Int64</span><span class="sxs-lookup"><span data-stu-id="d810c-110">Int64</span></span>  |
| <span data-ttu-id="d810c-111">warningIssued</span><span class="sxs-lookup"><span data-stu-id="d810c-111">warningIssued</span></span>         | <span data-ttu-id="d810c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d810c-112">Int64</span></span>  |
| <span data-ttu-id="d810c-113">sendProhibited</span><span class="sxs-lookup"><span data-stu-id="d810c-113">sendProhibited</span></span>        | <span data-ttu-id="d810c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d810c-114">Int64</span></span>  |
| <span data-ttu-id="d810c-115">sendReceiveProhibited</span><span class="sxs-lookup"><span data-stu-id="d810c-115">sendReceiveProhibited</span></span> | <span data-ttu-id="d810c-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d810c-116">Int64</span></span>  |
| <span data-ttu-id="d810c-117">尚</span><span class="sxs-lookup"><span data-stu-id="d810c-117">indeterminate</span></span>         | <span data-ttu-id="d810c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d810c-118">Int64</span></span>  |
| <span data-ttu-id="d810c-119">reportDate</span><span class="sxs-lookup"><span data-stu-id="d810c-119">reportDate</span></span>            | <span data-ttu-id="d810c-120">日期</span><span class="sxs-lookup"><span data-stu-id="d810c-120">Date</span></span>   |
| <span data-ttu-id="d810c-121">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d810c-121">reportPeriod</span></span>          | <span data-ttu-id="d810c-122">String</span><span class="sxs-lookup"><span data-stu-id="d810c-122">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d810c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d810c-123">JSON representation</span></span>

<span data-ttu-id="d810c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d810c-124">The following is a JSON representation of the resource.</span></span>

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
