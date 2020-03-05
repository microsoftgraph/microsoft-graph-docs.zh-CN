---
title: personType 资源类型
description: 表示人员类型。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 9b6dc5153fb12f44abad57d1977024675aa0bd45
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447190"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="ac140-103">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="ac140-103">personType resource type</span></span>

<span data-ttu-id="ac140-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ac140-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ac140-105">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="ac140-105">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac140-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac140-106">JSON representation</span></span>

<span data-ttu-id="ac140-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac140-107">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="ac140-108">属性</span><span class="sxs-lookup"><span data-stu-id="ac140-108">Properties</span></span>
| <span data-ttu-id="ac140-109">属性</span><span class="sxs-lookup"><span data-stu-id="ac140-109">Property</span></span>     | <span data-ttu-id="ac140-110">类型</span><span class="sxs-lookup"><span data-stu-id="ac140-110">Type</span></span>   |<span data-ttu-id="ac140-111">说明</span><span class="sxs-lookup"><span data-stu-id="ac140-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac140-112">class</span><span class="sxs-lookup"><span data-stu-id="ac140-112">class</span></span>|<span data-ttu-id="ac140-113">String</span><span class="sxs-lookup"><span data-stu-id="ac140-113">String</span></span>|<span data-ttu-id="ac140-114">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="ac140-114">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="ac140-115">subclass</span><span class="sxs-lookup"><span data-stu-id="ac140-115">subclass</span></span>|<span data-ttu-id="ac140-116">String</span><span class="sxs-lookup"><span data-stu-id="ac140-116">String</span></span>|<span data-ttu-id="ac140-117">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="ac140-117">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
