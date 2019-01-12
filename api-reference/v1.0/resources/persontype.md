---
title: personType 资源类型
description: 表示人员类型。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 270fa800242ae7a25ed0f5959a97b6a70f7cedd3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917270"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="5aec6-103">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="5aec6-103">personType resource type</span></span>

<span data-ttu-id="5aec6-104">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="5aec6-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5aec6-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aec6-105">JSON representation</span></span>

<span data-ttu-id="5aec6-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aec6-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5aec6-107">属性</span><span class="sxs-lookup"><span data-stu-id="5aec6-107">Properties</span></span>
| <span data-ttu-id="5aec6-108">属性</span><span class="sxs-lookup"><span data-stu-id="5aec6-108">Property</span></span>     | <span data-ttu-id="5aec6-109">类型</span><span class="sxs-lookup"><span data-stu-id="5aec6-109">Type</span></span>   |<span data-ttu-id="5aec6-110">说明</span><span class="sxs-lookup"><span data-stu-id="5aec6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5aec6-111">class</span><span class="sxs-lookup"><span data-stu-id="5aec6-111">class</span></span>|<span data-ttu-id="5aec6-112">String</span><span class="sxs-lookup"><span data-stu-id="5aec6-112">String</span></span>|<span data-ttu-id="5aec6-113">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="5aec6-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="5aec6-114">subclass</span><span class="sxs-lookup"><span data-stu-id="5aec6-114">subclass</span></span>|<span data-ttu-id="5aec6-115">String</span><span class="sxs-lookup"><span data-stu-id="5aec6-115">String</span></span>|<span data-ttu-id="5aec6-116">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="5aec6-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
