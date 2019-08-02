---
title: personType 资源类型
description: 表示人员类型。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 36310a469c5ed9289637f9701ce983db12b14fbf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035488"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="53e40-103">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="53e40-103">personType resource type</span></span>

<span data-ttu-id="53e40-104">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="53e40-104">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="53e40-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53e40-105">JSON representation</span></span>

<span data-ttu-id="53e40-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53e40-106">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="53e40-107">属性</span><span class="sxs-lookup"><span data-stu-id="53e40-107">Properties</span></span>
| <span data-ttu-id="53e40-108">属性</span><span class="sxs-lookup"><span data-stu-id="53e40-108">Property</span></span>     | <span data-ttu-id="53e40-109">类型</span><span class="sxs-lookup"><span data-stu-id="53e40-109">Type</span></span>   |<span data-ttu-id="53e40-110">说明</span><span class="sxs-lookup"><span data-stu-id="53e40-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="53e40-111">class</span><span class="sxs-lookup"><span data-stu-id="53e40-111">class</span></span>|<span data-ttu-id="53e40-112">String</span><span class="sxs-lookup"><span data-stu-id="53e40-112">String</span></span>|<span data-ttu-id="53e40-113">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="53e40-113">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="53e40-114">subclass</span><span class="sxs-lookup"><span data-stu-id="53e40-114">subclass</span></span>|<span data-ttu-id="53e40-115">String</span><span class="sxs-lookup"><span data-stu-id="53e40-115">String</span></span>|<span data-ttu-id="53e40-116">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="53e40-116">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
