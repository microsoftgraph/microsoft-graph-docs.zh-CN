---
title: personType 资源类型
description: 表示人员类型。
ms.openlocfilehash: 3938be8d1dd0bf4a4934de4bbcd7862185971128
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008418"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="a7a02-103">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7a02-103">personType resource type</span></span>

<span data-ttu-id="a7a02-104">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="a7a02-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a7a02-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7a02-105">JSON representation</span></span>

<span data-ttu-id="a7a02-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7a02-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a7a02-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7a02-107">Properties</span></span>
| <span data-ttu-id="a7a02-108">属性</span><span class="sxs-lookup"><span data-stu-id="a7a02-108">Property</span></span>     | <span data-ttu-id="a7a02-109">类型</span><span class="sxs-lookup"><span data-stu-id="a7a02-109">Type</span></span>   |<span data-ttu-id="a7a02-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7a02-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7a02-111">class</span><span class="sxs-lookup"><span data-stu-id="a7a02-111">class</span></span>|<span data-ttu-id="a7a02-112">String</span><span class="sxs-lookup"><span data-stu-id="a7a02-112">String</span></span>|<span data-ttu-id="a7a02-113">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="a7a02-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="a7a02-114">subclass</span><span class="sxs-lookup"><span data-stu-id="a7a02-114">subclass</span></span>|<span data-ttu-id="a7a02-115">String</span><span class="sxs-lookup"><span data-stu-id="a7a02-115">String</span></span>|<span data-ttu-id="a7a02-116">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="a7a02-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
