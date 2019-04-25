---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582162"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="1b0f0-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b0f0-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b0f0-104">描述在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1b0f0-105">属性</span><span class="sxs-lookup"><span data-stu-id="1b0f0-105">Properties</span></span>

| <span data-ttu-id="1b0f0-106">属性</span><span class="sxs-lookup"><span data-stu-id="1b0f0-106">Property</span></span>                   | <span data-ttu-id="1b0f0-107">类型</span><span class="sxs-lookup"><span data-stu-id="1b0f0-107">Type</span></span>                      | <span data-ttu-id="1b0f0-108">说明</span><span class="sxs-lookup"><span data-stu-id="1b0f0-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="1b0f0-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="1b0f0-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="1b0f0-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0f0-110">Boolean</span></span>                   |<span data-ttu-id="1b0f0-111">给定参数可多次提供 (例如, `Concatenate(string,string,...)`函数中的多个输入字符串)。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="1b0f0-112">name</span><span class="sxs-lookup"><span data-stu-id="1b0f0-112">name</span></span>                        |<span data-ttu-id="1b0f0-113">String</span><span class="sxs-lookup"><span data-stu-id="1b0f0-113">String</span></span>                    |<span data-ttu-id="1b0f0-114">参数名称。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-114">Parameter name.</span></span> |
|<span data-ttu-id="1b0f0-115">必需</span><span class="sxs-lookup"><span data-stu-id="1b0f0-115">required</span></span>                    |<span data-ttu-id="1b0f0-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0f0-116">Boolean</span></span>                   |<span data-ttu-id="1b0f0-117">`true`如果参数是必需的;否则`false`为。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="1b0f0-118">type</span><span class="sxs-lookup"><span data-stu-id="1b0f0-118">type</span></span>                        |<span data-ttu-id="1b0f0-119">String</span><span class="sxs-lookup"><span data-stu-id="1b0f0-119">String</span></span>                    |<span data-ttu-id="1b0f0-120">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="1b0f0-121">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b0f0-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b0f0-122">JSON representation</span></span>

<span data-ttu-id="1b0f0-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b0f0-123">The following is a JSON representation of the resource.</span></span>

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
