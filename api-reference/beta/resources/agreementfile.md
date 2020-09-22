---
title: agreementFile 资源类型
description: 表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否为默认文件) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 50663ca58323782a14b7e8c5681908aa5a108bdf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067487"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="555a8-104">agreementFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="555a8-104">agreementFile resource type</span></span>

<span data-ttu-id="555a8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="555a8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="555a8-106">表示租户使用 Azure Active Directory (Azure AD) 管理的可自定义使用条款协议文件。</span><span class="sxs-lookup"><span data-stu-id="555a8-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="555a8-107">它包含有关协议文件的元数据 (例如，名称、语言以及它是否为默认文件) 。</span><span class="sxs-lookup"><span data-stu-id="555a8-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="555a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="555a8-108">Properties</span></span>
| <span data-ttu-id="555a8-109">属性</span><span class="sxs-lookup"><span data-stu-id="555a8-109">Property</span></span>     | <span data-ttu-id="555a8-110">类型</span><span class="sxs-lookup"><span data-stu-id="555a8-110">Type</span></span>        | <span data-ttu-id="555a8-111">说明</span><span class="sxs-lookup"><span data-stu-id="555a8-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="555a8-112">fileData</span><span class="sxs-lookup"><span data-stu-id="555a8-112">fileData</span></span>|[<span data-ttu-id="555a8-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="555a8-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="555a8-114">代表使用条款的 PDF 文档的数据。</span><span class="sxs-lookup"><span data-stu-id="555a8-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="555a8-115">只读。</span><span class="sxs-lookup"><span data-stu-id="555a8-115">Read-only.</span></span>|
|<span data-ttu-id="555a8-116">fileName</span><span class="sxs-lookup"><span data-stu-id="555a8-116">fileName</span></span>|<span data-ttu-id="555a8-117">String</span><span class="sxs-lookup"><span data-stu-id="555a8-117">String</span></span>|<span data-ttu-id="555a8-118">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="555a8-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="555a8-119">只读。</span><span class="sxs-lookup"><span data-stu-id="555a8-119">Read-only.</span></span>|
|<span data-ttu-id="555a8-120">id</span><span class="sxs-lookup"><span data-stu-id="555a8-120">id</span></span>|<span data-ttu-id="555a8-121">String</span><span class="sxs-lookup"><span data-stu-id="555a8-121">String</span></span>|<span data-ttu-id="555a8-122">只读。</span><span class="sxs-lookup"><span data-stu-id="555a8-122">Read-only.</span></span>|
|<span data-ttu-id="555a8-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="555a8-123">isDefault</span></span>|<span data-ttu-id="555a8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="555a8-124">Boolean</span></span>|<span data-ttu-id="555a8-125">指示是否为默认协议文件（如果没有任何区域性与客户端首选项匹配）。</span><span class="sxs-lookup"><span data-stu-id="555a8-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="555a8-126">如果没有任何文件被标记为默认值，则第一个文件将被视为默认值。</span><span class="sxs-lookup"><span data-stu-id="555a8-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="555a8-127">只读。</span><span class="sxs-lookup"><span data-stu-id="555a8-127">Read-only.</span></span>|
|<span data-ttu-id="555a8-128">language</span><span class="sxs-lookup"><span data-stu-id="555a8-128">language</span></span>|<span data-ttu-id="555a8-129">String</span><span class="sxs-lookup"><span data-stu-id="555a8-129">String</span></span>|<span data-ttu-id="555a8-130">协议文件的区域性（格式为 languagecode2/regioncode2）。</span><span class="sxs-lookup"><span data-stu-id="555a8-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="555a8-131">languagecode2 是从 ISO 639-1 派生的一个由两个小写字母组成的代码。</span><span class="sxs-lookup"><span data-stu-id="555a8-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="555a8-132">国家/regioncode2 派生自 ISO 3166，通常包含两个大写字母或一个 BCP-47 语言标记 (例如 en-us) 。</span><span class="sxs-lookup"><span data-stu-id="555a8-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="555a8-133">只读。</span><span class="sxs-lookup"><span data-stu-id="555a8-133">Read-only.</span></span>|


<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="555a8-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="555a8-134">JSON representation</span></span>

<span data-ttu-id="555a8-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="555a8-135">The following is a JSON representation of the resource.</span></span>

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


