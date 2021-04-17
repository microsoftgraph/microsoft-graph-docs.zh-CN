---
title: assignmentOrder 资源类型
description: 定义在用户流中收集的属性的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c5faed250c07d5c4416c91a5452f1276c6b728e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882827"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="bdfaa-103">assignmentOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdfaa-103">assignmentOrder resource type</span></span>

<span data-ttu-id="bdfaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdfaa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bdfaa-105">用于定义在用户流中收集的属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="bdfaa-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="bdfaa-106">顺序确定当用户使用用户流注册时属性集合页的显示方式。</span><span class="sxs-lookup"><span data-stu-id="bdfaa-106">The order determines how the attribute collection page is displayed when a user signs up using a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="bdfaa-107">属性</span><span class="sxs-lookup"><span data-stu-id="bdfaa-107">Properties</span></span>

|<span data-ttu-id="bdfaa-108">属性</span><span class="sxs-lookup"><span data-stu-id="bdfaa-108">Property</span></span>|<span data-ttu-id="bdfaa-109">类型</span><span class="sxs-lookup"><span data-stu-id="bdfaa-109">Type</span></span>|<span data-ttu-id="bdfaa-110">说明</span><span class="sxs-lookup"><span data-stu-id="bdfaa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdfaa-111">order</span><span class="sxs-lookup"><span data-stu-id="bdfaa-111">order</span></span>|<span data-ttu-id="bdfaa-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="bdfaa-112">String collection</span></span>|<span data-ttu-id="bdfaa-113">identityUserFlowAttribute 对象标识符的列表，这些标识符确定应在用户流中收集属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="bdfaa-113">A list of identityUserFlowAttribute object identifiers that determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdfaa-114">关系</span><span class="sxs-lookup"><span data-stu-id="bdfaa-114">Relationships</span></span>

<span data-ttu-id="bdfaa-115">无。</span><span class="sxs-lookup"><span data-stu-id="bdfaa-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bdfaa-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdfaa-116">JSON representation</span></span>

<span data-ttu-id="bdfaa-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdfaa-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.assignmentOrder",
  "order": [
    "String"
  ]
}
```
