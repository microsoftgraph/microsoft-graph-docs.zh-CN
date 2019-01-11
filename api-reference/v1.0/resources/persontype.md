---
title: personType 资源类型
description: 表示人员类型。
localization_priority: Normal
ms.openlocfilehash: d30441a9eab3f51b63e31e5c3c627444312449ba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831491"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="92e90-103">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="92e90-103">personType resource type</span></span>

<span data-ttu-id="92e90-104">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="92e90-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="92e90-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92e90-105">JSON representation</span></span>

<span data-ttu-id="92e90-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92e90-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="92e90-107">属性</span><span class="sxs-lookup"><span data-stu-id="92e90-107">Properties</span></span>
| <span data-ttu-id="92e90-108">属性</span><span class="sxs-lookup"><span data-stu-id="92e90-108">Property</span></span>     | <span data-ttu-id="92e90-109">类型</span><span class="sxs-lookup"><span data-stu-id="92e90-109">Type</span></span>   |<span data-ttu-id="92e90-110">说明</span><span class="sxs-lookup"><span data-stu-id="92e90-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92e90-111">class</span><span class="sxs-lookup"><span data-stu-id="92e90-111">class</span></span>|<span data-ttu-id="92e90-112">String</span><span class="sxs-lookup"><span data-stu-id="92e90-112">String</span></span>|<span data-ttu-id="92e90-113">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="92e90-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="92e90-114">subclass</span><span class="sxs-lookup"><span data-stu-id="92e90-114">subclass</span></span>|<span data-ttu-id="92e90-115">String</span><span class="sxs-lookup"><span data-stu-id="92e90-115">String</span></span>|<span data-ttu-id="92e90-116">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="92e90-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
