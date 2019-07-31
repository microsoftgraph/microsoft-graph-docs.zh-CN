---
title: agreementFile 资源类型
description: 表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。 它包含有关协议文件的元数据 (例如, 名称、语言以及它是否为默认文件)。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a6651eafb57d75d6edb6342bd3f382008336332c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974518"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="6a300-104">agreementFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a300-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a300-105">表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。</span><span class="sxs-lookup"><span data-stu-id="6a300-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="6a300-106">它包含有关协议文件的元数据 (例如, 名称、语言以及它是否为默认文件)。</span><span class="sxs-lookup"><span data-stu-id="6a300-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="6a300-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a300-107">Properties</span></span>
| <span data-ttu-id="6a300-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a300-108">Property</span></span>     | <span data-ttu-id="6a300-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a300-109">Type</span></span>        | <span data-ttu-id="6a300-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a300-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6a300-111">fileData</span><span class="sxs-lookup"><span data-stu-id="6a300-111">fileData</span></span>|[<span data-ttu-id="6a300-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="6a300-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="6a300-113">代表使用条款的 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="6a300-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="6a300-114">只读。</span><span class="sxs-lookup"><span data-stu-id="6a300-114">Read-only.</span></span>|
|<span data-ttu-id="6a300-115">fileName</span><span class="sxs-lookup"><span data-stu-id="6a300-115">fileName</span></span>|<span data-ttu-id="6a300-116">String</span><span class="sxs-lookup"><span data-stu-id="6a300-116">String</span></span>|<span data-ttu-id="6a300-117">协议文件的名称 (例如, TOU)。</span><span class="sxs-lookup"><span data-stu-id="6a300-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="6a300-118">只读。</span><span class="sxs-lookup"><span data-stu-id="6a300-118">Read-only.</span></span>|
|<span data-ttu-id="6a300-119">id</span><span class="sxs-lookup"><span data-stu-id="6a300-119">id</span></span>|<span data-ttu-id="6a300-120">String</span><span class="sxs-lookup"><span data-stu-id="6a300-120">String</span></span>|<span data-ttu-id="6a300-121">只读。</span><span class="sxs-lookup"><span data-stu-id="6a300-121">Read-only.</span></span>|
|<span data-ttu-id="6a300-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="6a300-122">isDefault</span></span>|<span data-ttu-id="6a300-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a300-123">Boolean</span></span>|<span data-ttu-id="6a300-124">指示是否为默认协议文件 (如果没有任何区域性与客户端首选项匹配)。</span><span class="sxs-lookup"><span data-stu-id="6a300-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="6a300-125">如果没有任何文件被标记为默认值, 则第一个文件将被视为默认值。</span><span class="sxs-lookup"><span data-stu-id="6a300-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="6a300-126">只读。</span><span class="sxs-lookup"><span data-stu-id="6a300-126">Read-only.</span></span>|
|<span data-ttu-id="6a300-127">language</span><span class="sxs-lookup"><span data-stu-id="6a300-127">language</span></span>|<span data-ttu-id="6a300-128">String</span><span class="sxs-lookup"><span data-stu-id="6a300-128">String</span></span>|<span data-ttu-id="6a300-129">协议文件的区域性 (格式为 languagecode2/regioncode2)。</span><span class="sxs-lookup"><span data-stu-id="6a300-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="6a300-130">languagecode2 是从 ISO 639-1 派生的一个由两个小写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="6a300-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="6a300-131">国家/regioncode2 派生自 ISO 3166, 通常包含两个大写字母或一个 BCP-47 语言标记 (例如 en-us)。</span><span class="sxs-lookup"><span data-stu-id="6a300-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="6a300-132">只读。</span><span class="sxs-lookup"><span data-stu-id="6a300-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a300-133">关系</span><span class="sxs-lookup"><span data-stu-id="6a300-133">Relationships</span></span>
<span data-ttu-id="6a300-134">无。</span><span class="sxs-lookup"><span data-stu-id="6a300-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6a300-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a300-135">JSON representation</span></span>

<span data-ttu-id="6a300-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a300-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
