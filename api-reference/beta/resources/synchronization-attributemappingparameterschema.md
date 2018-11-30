---
title: attributeMappingParameterSchema 资源类型
description: 介绍在 attributeMappingFunctionSchema 中使用的单个参数。
ms.openlocfilehash: 164387a345f245f390d24b89a349e02ee2242041
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048170"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="566cc-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="566cc-103">attributeMappingParameterSchema resource type</span></span>

> <span data-ttu-id="566cc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="566cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="566cc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="566cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="566cc-106">介绍在[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="566cc-106">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="566cc-107">属性</span><span class="sxs-lookup"><span data-stu-id="566cc-107">Properties</span></span>

| <span data-ttu-id="566cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="566cc-108">Property</span></span>                   | <span data-ttu-id="566cc-109">类型</span><span class="sxs-lookup"><span data-stu-id="566cc-109">Type</span></span>                      | <span data-ttu-id="566cc-110">说明</span><span class="sxs-lookup"><span data-stu-id="566cc-110">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="566cc-111">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="566cc-111">allowMultipleOccurrences</span></span>    |<span data-ttu-id="566cc-112">布尔</span><span class="sxs-lookup"><span data-stu-id="566cc-112">Boolean</span></span>                   |<span data-ttu-id="566cc-113">给定的参数可提供多次 (多个输入中的字符串，如`Concatenate(string,string,...)`函数)。</span><span class="sxs-lookup"><span data-stu-id="566cc-113">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="566cc-114">name</span><span class="sxs-lookup"><span data-stu-id="566cc-114">name</span></span>                        |<span data-ttu-id="566cc-115">字符串</span><span class="sxs-lookup"><span data-stu-id="566cc-115">String</span></span>                    |<span data-ttu-id="566cc-116">参数名称。</span><span class="sxs-lookup"><span data-stu-id="566cc-116">Parameter name.</span></span> |
|<span data-ttu-id="566cc-117">必需</span><span class="sxs-lookup"><span data-stu-id="566cc-117">required</span></span>                    |<span data-ttu-id="566cc-118">布尔</span><span class="sxs-lookup"><span data-stu-id="566cc-118">Boolean</span></span>                   |<span data-ttu-id="566cc-119">`true`如果该参数是必需的;否则为`false`。</span><span class="sxs-lookup"><span data-stu-id="566cc-119">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="566cc-120">type</span><span class="sxs-lookup"><span data-stu-id="566cc-120">type</span></span>                        |<span data-ttu-id="566cc-121">String</span><span class="sxs-lookup"><span data-stu-id="566cc-121">String</span></span>                    |<span data-ttu-id="566cc-122">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="566cc-122">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="566cc-123">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="566cc-123">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="566cc-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="566cc-124">JSON representation</span></span>

<span data-ttu-id="566cc-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="566cc-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->