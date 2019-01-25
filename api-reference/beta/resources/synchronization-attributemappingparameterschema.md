---
title: attributeMappingParameterSchema 资源类型
description: 介绍在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529948"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="ed200-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed200-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed200-104">介绍在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="ed200-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ed200-105">属性</span><span class="sxs-lookup"><span data-stu-id="ed200-105">Properties</span></span>

| <span data-ttu-id="ed200-106">属性</span><span class="sxs-lookup"><span data-stu-id="ed200-106">Property</span></span>                   | <span data-ttu-id="ed200-107">类型</span><span class="sxs-lookup"><span data-stu-id="ed200-107">Type</span></span>                      | <span data-ttu-id="ed200-108">说明</span><span class="sxs-lookup"><span data-stu-id="ed200-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="ed200-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="ed200-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="ed200-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed200-110">Boolean</span></span>                   |<span data-ttu-id="ed200-111">给定的参数可提供多次 (多个输入中的字符串，如`Concatenate(string,string,...)`函数)。</span><span class="sxs-lookup"><span data-stu-id="ed200-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="ed200-112">name</span><span class="sxs-lookup"><span data-stu-id="ed200-112">name</span></span>                        |<span data-ttu-id="ed200-113">String</span><span class="sxs-lookup"><span data-stu-id="ed200-113">String</span></span>                    |<span data-ttu-id="ed200-114">参数名称</span><span class="sxs-lookup"><span data-stu-id="ed200-114">Parameter name.</span></span> |
|<span data-ttu-id="ed200-115">必需</span><span class="sxs-lookup"><span data-stu-id="ed200-115">required</span></span>                    |<span data-ttu-id="ed200-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ed200-116">Boolean</span></span>                   |<span data-ttu-id="ed200-117">`true`如果该参数是必需的;否则为`false`。</span><span class="sxs-lookup"><span data-stu-id="ed200-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="ed200-118">type</span><span class="sxs-lookup"><span data-stu-id="ed200-118">type</span></span>                        |<span data-ttu-id="ed200-119">String</span><span class="sxs-lookup"><span data-stu-id="ed200-119">String</span></span>                    |<span data-ttu-id="ed200-120">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="ed200-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="ed200-121">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="ed200-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed200-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed200-122">JSON representation</span></span>

<span data-ttu-id="ed200-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed200-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
