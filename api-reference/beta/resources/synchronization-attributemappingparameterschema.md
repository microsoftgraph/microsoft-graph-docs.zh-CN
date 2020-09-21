---
title: attributeMappingParameterSchema 资源类型
description: 描述在 attributeMappingFunctionSchema 中使用的单个参数。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32710c5411f054ad096bdd293a2f7d46e89a6944
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078073"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="11c4e-103">attributeMappingParameterSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="11c4e-103">attributeMappingParameterSchema resource type</span></span>

<span data-ttu-id="11c4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11c4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11c4e-105">描述在 [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)中使用的单个参数。</span><span class="sxs-lookup"><span data-stu-id="11c4e-105">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11c4e-106">属性</span><span class="sxs-lookup"><span data-stu-id="11c4e-106">Properties</span></span>

| <span data-ttu-id="11c4e-107">属性</span><span class="sxs-lookup"><span data-stu-id="11c4e-107">Property</span></span>                   | <span data-ttu-id="11c4e-108">类型</span><span class="sxs-lookup"><span data-stu-id="11c4e-108">Type</span></span>                      | <span data-ttu-id="11c4e-109">说明</span><span class="sxs-lookup"><span data-stu-id="11c4e-109">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="11c4e-110">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="11c4e-110">allowMultipleOccurrences</span></span>    |<span data-ttu-id="11c4e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c4e-111">Boolean</span></span>                   |<span data-ttu-id="11c4e-112">可以多次提供给定参数 (例如，函数中的多个输入字符串 `Concatenate(string,string,...)`) 。</span><span class="sxs-lookup"><span data-stu-id="11c4e-112">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="11c4e-113">名称</span><span class="sxs-lookup"><span data-stu-id="11c4e-113">name</span></span>                        |<span data-ttu-id="11c4e-114">String</span><span class="sxs-lookup"><span data-stu-id="11c4e-114">String</span></span>                    |<span data-ttu-id="11c4e-115">参数名称。</span><span class="sxs-lookup"><span data-stu-id="11c4e-115">Parameter name.</span></span> |
|<span data-ttu-id="11c4e-116">必需</span><span class="sxs-lookup"><span data-stu-id="11c4e-116">required</span></span>                    |<span data-ttu-id="11c4e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="11c4e-117">Boolean</span></span>                   |<span data-ttu-id="11c4e-118">`true` 如果参数是必需的;否则为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="11c4e-118">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="11c4e-119">type</span><span class="sxs-lookup"><span data-stu-id="11c4e-119">type</span></span>                        |<span data-ttu-id="11c4e-120">String</span><span class="sxs-lookup"><span data-stu-id="11c4e-120">String</span></span>                    |<span data-ttu-id="11c4e-121">可取值为：`Boolean`、`Binary`、`Reference`、`Integer` 或 `String`。</span><span class="sxs-lookup"><span data-stu-id="11c4e-121">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="11c4e-122">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="11c4e-122">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11c4e-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11c4e-123">JSON representation</span></span>

<span data-ttu-id="11c4e-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11c4e-124">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


