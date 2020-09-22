---
title: personType 资源类型
description: 表示人员类型。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cc8a2c3bac3fab1a7dd9f94cc512de9172481aeb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022825"
---
# <a name="persontype-resource-type"></a><span data-ttu-id="053fc-103">personType 资源类型</span><span class="sxs-lookup"><span data-stu-id="053fc-103">personType resource type</span></span>

<span data-ttu-id="053fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="053fc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="053fc-105">表示人员类型。</span><span class="sxs-lookup"><span data-stu-id="053fc-105">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="053fc-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="053fc-106">JSON representation</span></span>

<span data-ttu-id="053fc-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="053fc-107">The following is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="053fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="053fc-108">Properties</span></span>
| <span data-ttu-id="053fc-109">属性</span><span class="sxs-lookup"><span data-stu-id="053fc-109">Property</span></span>     | <span data-ttu-id="053fc-110">类型</span><span class="sxs-lookup"><span data-stu-id="053fc-110">Type</span></span>   |<span data-ttu-id="053fc-111">说明</span><span class="sxs-lookup"><span data-stu-id="053fc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="053fc-112">class</span><span class="sxs-lookup"><span data-stu-id="053fc-112">class</span></span>|<span data-ttu-id="053fc-113">String</span><span class="sxs-lookup"><span data-stu-id="053fc-113">String</span></span>|<span data-ttu-id="053fc-114">数据源的类型，例如 Person。</span><span class="sxs-lookup"><span data-stu-id="053fc-114">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="053fc-115">subclass</span><span class="sxs-lookup"><span data-stu-id="053fc-115">subclass</span></span>|<span data-ttu-id="053fc-116">String</span><span class="sxs-lookup"><span data-stu-id="053fc-116">String</span></span>|<span data-ttu-id="053fc-117">数据源的次要类型，例如 OrganizationUser。</span><span class="sxs-lookup"><span data-stu-id="053fc-117">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

