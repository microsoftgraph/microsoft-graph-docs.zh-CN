---
title: assignmentOrder 资源类型
description: 用于定义在用户流中收集的属性的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41b75e1adf5459279b5675278a8f00a82110b457
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581288"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="cc215-103">assignmentOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc215-103">assignmentOrder resource type</span></span>

<span data-ttu-id="cc215-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc215-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc215-105">用于定义在用户流中收集的属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="cc215-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="cc215-106">这将确定当用户通过用户流注册时，如何显示属性集合页。</span><span class="sxs-lookup"><span data-stu-id="cc215-106">THis determines how the attribute collection page is displayed when a user signs up via a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="cc215-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc215-107">Properties</span></span>

|<span data-ttu-id="cc215-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc215-108">Property</span></span>|<span data-ttu-id="cc215-109">类型</span><span class="sxs-lookup"><span data-stu-id="cc215-109">Type</span></span>|<span data-ttu-id="cc215-110">Description</span><span class="sxs-lookup"><span data-stu-id="cc215-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc215-111">顺序</span><span class="sxs-lookup"><span data-stu-id="cc215-111">order</span></span>|<span data-ttu-id="cc215-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="cc215-112">String collection</span></span>|<span data-ttu-id="cc215-113">提供的 identityUserFlowAttribute Id 的列表，用于确定应在用户流中收集属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="cc215-113">A list of identityUserFlowAttribute IDs provided to determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc215-114">关系</span><span class="sxs-lookup"><span data-stu-id="cc215-114">Relationships</span></span>

<span data-ttu-id="cc215-115">无。</span><span class="sxs-lookup"><span data-stu-id="cc215-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc215-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc215-116">JSON representation</span></span>

<span data-ttu-id="cc215-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc215-117">The following is a JSON representation of the resource.</span></span>
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
