---
title: assignmentOrder 资源类型
description: 用于定义在用户流中收集的属性的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7d7716cb4b13917aad33cd88afeb364a2891e3df
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761238"
---
# <a name="assignmentorder-resource-type"></a><span data-ttu-id="fb401-103">assignmentOrder 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb401-103">assignmentOrder resource type</span></span>

<span data-ttu-id="fb401-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb401-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fb401-105">用于定义在用户流中收集的属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="fb401-105">Used to define the order of the attributes being collected within a user flow.</span></span> <span data-ttu-id="fb401-106">THis 确定当用户通过用户流注册时属性集合页的显示方式。</span><span class="sxs-lookup"><span data-stu-id="fb401-106">THis determines how the attribute collection page is displayed when a user signs up via a user flow.</span></span>

## <a name="properties"></a><span data-ttu-id="fb401-107">属性</span><span class="sxs-lookup"><span data-stu-id="fb401-107">Properties</span></span>

|<span data-ttu-id="fb401-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb401-108">Property</span></span>|<span data-ttu-id="fb401-109">类型</span><span class="sxs-lookup"><span data-stu-id="fb401-109">Type</span></span>|<span data-ttu-id="fb401-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb401-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb401-111">order</span><span class="sxs-lookup"><span data-stu-id="fb401-111">order</span></span>|<span data-ttu-id="fb401-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="fb401-112">String collection</span></span>|<span data-ttu-id="fb401-113">提供的 identityUserFlowAttribute ID 列表，用于确定应在用户流中收集属性的顺序。</span><span class="sxs-lookup"><span data-stu-id="fb401-113">A list of identityUserFlowAttribute IDs provided to determine the order in which attributes should be collected within a user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb401-114">关系</span><span class="sxs-lookup"><span data-stu-id="fb401-114">Relationships</span></span>

<span data-ttu-id="fb401-115">无。</span><span class="sxs-lookup"><span data-stu-id="fb401-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb401-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb401-116">JSON representation</span></span>

<span data-ttu-id="fb401-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb401-117">The following is a JSON representation of the resource.</span></span>
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
