---
title: agreementFileLocalization 资源类型
description: 表示 Azure Active Directory 中许可协议的本地化策略文件 (Azure AD) 。 它包含有关协议文件的元数据 (例如，名称、语言以及它是否是默认文件) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: fab48421542d8ad27ec9bc584d8728a4acb340a4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720756"
---
# <a name="agreementfilelocalization-resource-type"></a><span data-ttu-id="adfa3-104">agreementFileLocalization 资源类型</span><span class="sxs-lookup"><span data-stu-id="adfa3-104">agreementFileLocalization resource type</span></span>

<span data-ttu-id="adfa3-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adfa3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adfa3-106">表示租户使用 Azure AD (Azure Active Directory 管理) 。</span><span class="sxs-lookup"><span data-stu-id="adfa3-106">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="adfa3-107">它包含有关协议文件的元数据 (例如，名称、语言以及它是否是默认文件) 。</span><span class="sxs-lookup"><span data-stu-id="adfa3-107">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Create agreementFileLocalization](../api/agreementfilelocalization-post-agreementfilelocalizations.md) | [agreementfilelocalization](agreementfilelocalization.md) | Create a new agreementFileLocalization. |
| [List agreementFileLocalizations](../api/agreementfilelocalization-list.md) | [agreementfilelocalization](agreementfilelocalization.md) collection | Get an agreementFileLocalization object collection. |
| [Get agreementFileLocalization](../api/agreementfilelocalization-get.md) | [agreementfilelocalization](agreementfilelocalization.md) | Read properties and relationships of an agreementFileLocalization object. |
| [List agreementFileVersions](../api/agreementfileversion-list.md) | [agreementfileversion](agreementfileversion.md) collection | Get an agreementFileVersion object collection. |
| [Get agreementFileVersion](../api/agreementfileversion-get.md) | [agreementfileversion](agreementfileversion.md) | Read properties and relationships of an agreementFileVersion object. |
-->

## <a name="properties"></a><span data-ttu-id="adfa3-108">属性</span><span class="sxs-lookup"><span data-stu-id="adfa3-108">Properties</span></span>
| <span data-ttu-id="adfa3-109">属性</span><span class="sxs-lookup"><span data-stu-id="adfa3-109">Property</span></span>     | <span data-ttu-id="adfa3-110">类型</span><span class="sxs-lookup"><span data-stu-id="adfa3-110">Type</span></span>        | <span data-ttu-id="adfa3-111">说明</span><span class="sxs-lookup"><span data-stu-id="adfa3-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="adfa3-112">fileData</span><span class="sxs-lookup"><span data-stu-id="adfa3-112">fileData</span></span>|[<span data-ttu-id="adfa3-113">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="adfa3-113">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="adfa3-114">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="adfa3-114">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="adfa3-115">只读。</span><span class="sxs-lookup"><span data-stu-id="adfa3-115">Read-only.</span></span>|
|<span data-ttu-id="adfa3-116">fileName</span><span class="sxs-lookup"><span data-stu-id="adfa3-116">fileName</span></span>|<span data-ttu-id="adfa3-117">String</span><span class="sxs-lookup"><span data-stu-id="adfa3-117">String</span></span>|<span data-ttu-id="adfa3-118">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="adfa3-118">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="adfa3-119">只读。</span><span class="sxs-lookup"><span data-stu-id="adfa3-119">Read-only.</span></span>|
|<span data-ttu-id="adfa3-120">id</span><span class="sxs-lookup"><span data-stu-id="adfa3-120">id</span></span>|<span data-ttu-id="adfa3-121">String</span><span class="sxs-lookup"><span data-stu-id="adfa3-121">String</span></span>|<span data-ttu-id="adfa3-122">只读。</span><span class="sxs-lookup"><span data-stu-id="adfa3-122">Read-only.</span></span>|
|<span data-ttu-id="adfa3-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="adfa3-123">isDefault</span></span>|<span data-ttu-id="adfa3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="adfa3-124">Boolean</span></span>|<span data-ttu-id="adfa3-125">指示如果没有任何区域性与客户端首选项匹配，则此文件是否是默认协议文件。</span><span class="sxs-lookup"><span data-stu-id="adfa3-125">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="adfa3-126">如果没有将任何文件标记为默认文件，则第一个文件将被视为默认文件。</span><span class="sxs-lookup"><span data-stu-id="adfa3-126">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="adfa3-127">只读。</span><span class="sxs-lookup"><span data-stu-id="adfa3-127">Read-only.</span></span>|
|<span data-ttu-id="adfa3-128">language</span><span class="sxs-lookup"><span data-stu-id="adfa3-128">language</span></span>|<span data-ttu-id="adfa3-129">String</span><span class="sxs-lookup"><span data-stu-id="adfa3-129">String</span></span>|<span data-ttu-id="adfa3-130">语言代码2-country/regioncode2 格式的协议文件的区域性。</span><span class="sxs-lookup"><span data-stu-id="adfa3-130">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="adfa3-131">languagecode2 是派生自 ISO 639-1 的两个字母小写代码。</span><span class="sxs-lookup"><span data-stu-id="adfa3-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="adfa3-132">country/regioncode2 派生自 ISO 3166，通常由两个大写字母或 BCP-47 语言标记 (例如 en-US) 。</span><span class="sxs-lookup"><span data-stu-id="adfa3-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="adfa3-133">只读。</span><span class="sxs-lookup"><span data-stu-id="adfa3-133">Read-only.</span></span>|
|<span data-ttu-id="adfa3-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="adfa3-134">isMajorVersion</span></span>|<span data-ttu-id="adfa3-135">布尔</span><span class="sxs-lookup"><span data-stu-id="adfa3-135">Boolean</span></span>|<span data-ttu-id="adfa3-136">指示协议文件是否是主要版本更新。</span><span class="sxs-lookup"><span data-stu-id="adfa3-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="adfa3-137">主要版本更新使协议对相应语言的接受无效。</span><span class="sxs-lookup"><span data-stu-id="adfa3-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="adfa3-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adfa3-138">createdDateTime</span></span>|<span data-ttu-id="adfa3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adfa3-139">DateTimeOffset</span></span>|<span data-ttu-id="adfa3-140">表示文件创建时间的日期时间。</span><span class="sxs-lookup"><span data-stu-id="adfa3-140">The date time representing when the file was created.</span></span> <span data-ttu-id="adfa3-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="adfa3-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adfa3-142">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="adfa3-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|versions|[agreementFileVersion](agreementfileversion.md) collection|The version history for the localized agreement file.|
-->

## <a name="json-representation"></a><span data-ttu-id="adfa3-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adfa3-143">JSON representation</span></span>

<span data-ttu-id="adfa3-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adfa3-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileLocalization"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": "Boolean",
  "language": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileLocalization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
