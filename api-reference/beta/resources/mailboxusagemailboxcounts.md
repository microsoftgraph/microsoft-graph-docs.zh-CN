---
title: mailboxUsageMailboxCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 41bb58fa74deb9f8296a8f109d83b7cdeb73012e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522846"
---
# <a name="mailboxusagemailboxcounts-resource-type"></a><span data-ttu-id="a66fd-103">mailboxUsageMailboxCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a66fd-103">mailboxUsageMailboxCounts resource type</span></span>

<span data-ttu-id="a66fd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a66fd-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a66fd-105">属性</span><span class="sxs-lookup"><span data-stu-id="a66fd-105">Properties</span></span>

| <span data-ttu-id="a66fd-106">属性</span><span class="sxs-lookup"><span data-stu-id="a66fd-106">Property</span></span>          | <span data-ttu-id="a66fd-107">类型</span><span class="sxs-lookup"><span data-stu-id="a66fd-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="a66fd-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a66fd-108">reportRefreshDate</span></span> | <span data-ttu-id="a66fd-109">日期</span><span class="sxs-lookup"><span data-stu-id="a66fd-109">Date</span></span>   |
| <span data-ttu-id="a66fd-110">total</span><span class="sxs-lookup"><span data-stu-id="a66fd-110">total</span></span>             | <span data-ttu-id="a66fd-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a66fd-111">Int64</span></span>  |
| <span data-ttu-id="a66fd-112">工作</span><span class="sxs-lookup"><span data-stu-id="a66fd-112">active</span></span>            | <span data-ttu-id="a66fd-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a66fd-113">Int64</span></span>  |
| <span data-ttu-id="a66fd-114">reportDate</span><span class="sxs-lookup"><span data-stu-id="a66fd-114">reportDate</span></span>        | <span data-ttu-id="a66fd-115">日期</span><span class="sxs-lookup"><span data-stu-id="a66fd-115">Date</span></span>   |
| <span data-ttu-id="a66fd-116">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a66fd-116">reportPeriod</span></span>      | <span data-ttu-id="a66fd-117">String</span><span class="sxs-lookup"><span data-stu-id="a66fd-117">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a66fd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a66fd-118">JSON representation</span></span>

<span data-ttu-id="a66fd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a66fd-119">The following is a JSON representation of the resource.</span></span>

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
