---
title: siteActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
author: ''
ms.openlocfilehash: 0e24da683b2abe319a60e5a51144a96f9ec00135
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520546"
---
# <a name="siteactivitysummary-resource-type"></a><span data-ttu-id="b8498-103">siteActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8498-103">siteActivitySummary resource type</span></span>

<span data-ttu-id="b8498-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b8498-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="b8498-105">属性</span><span class="sxs-lookup"><span data-stu-id="b8498-105">Properties</span></span>

| <span data-ttu-id="b8498-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8498-106">Property</span></span>          | <span data-ttu-id="b8498-107">类型</span><span class="sxs-lookup"><span data-stu-id="b8498-107">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="b8498-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="b8498-108">reportRefreshDate</span></span> | <span data-ttu-id="b8498-109">日期</span><span class="sxs-lookup"><span data-stu-id="b8498-109">Date</span></span>   |
| <span data-ttu-id="b8498-110">viewedOrEdited</span><span class="sxs-lookup"><span data-stu-id="b8498-110">viewedOrEdited</span></span>    | <span data-ttu-id="b8498-111">Int64</span><span class="sxs-lookup"><span data-stu-id="b8498-111">Int64</span></span>  |
| <span data-ttu-id="b8498-112">保持</span><span class="sxs-lookup"><span data-stu-id="b8498-112">synced</span></span>            | <span data-ttu-id="b8498-113">Int64</span><span class="sxs-lookup"><span data-stu-id="b8498-113">Int64</span></span>  |
| <span data-ttu-id="b8498-114">sharedInternally</span><span class="sxs-lookup"><span data-stu-id="b8498-114">sharedInternally</span></span>  | <span data-ttu-id="b8498-115">Int64</span><span class="sxs-lookup"><span data-stu-id="b8498-115">Int64</span></span>  |
| <span data-ttu-id="b8498-116">sharedExternally</span><span class="sxs-lookup"><span data-stu-id="b8498-116">sharedExternally</span></span>  | <span data-ttu-id="b8498-117">Int64</span><span class="sxs-lookup"><span data-stu-id="b8498-117">Int64</span></span>  |
| <span data-ttu-id="b8498-118">reportDate</span><span class="sxs-lookup"><span data-stu-id="b8498-118">reportDate</span></span>        | <span data-ttu-id="b8498-119">日期</span><span class="sxs-lookup"><span data-stu-id="b8498-119">Date</span></span>   |
| <span data-ttu-id="b8498-120">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="b8498-120">reportPeriod</span></span>      | <span data-ttu-id="b8498-121">String</span><span class="sxs-lookup"><span data-stu-id="b8498-121">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b8498-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8498-122">JSON representation</span></span>

<span data-ttu-id="b8498-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8498-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "viewedOrEdited": 1024, 
  "synced": 1024, 
  "sharedInternally": 1024, 
  "sharedExternally": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
