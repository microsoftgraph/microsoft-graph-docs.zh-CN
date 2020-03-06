---
author: daspek
ms.author: dspektor
title: incompleteData 资源类型
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5fdf78b0fdb0a34e87296619c477d9f868d0756e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531324"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="8f081-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f081-103">incompleteData resource type</span></span>

<span data-ttu-id="8f081-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f081-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f081-105">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="8f081-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="8f081-106">中的属性可能提供有关数据不完整的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="8f081-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="8f081-107">属性</span><span class="sxs-lookup"><span data-stu-id="8f081-107">Properties</span></span>

| <span data-ttu-id="8f081-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f081-108">Property</span></span>                  | <span data-ttu-id="8f081-109">类型</span><span class="sxs-lookup"><span data-stu-id="8f081-109">Type</span></span>           | <span data-ttu-id="8f081-110">说明</span><span class="sxs-lookup"><span data-stu-id="8f081-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="8f081-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="8f081-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="8f081-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f081-112">DateTimeOffset</span></span> | <span data-ttu-id="8f081-113">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="8f081-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="8f081-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="8f081-114">wasThrottled</span></span>              | <span data-ttu-id="8f081-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f081-115">Boolean</span></span>        | <span data-ttu-id="8f081-116">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="8f081-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f081-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f081-117">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->
