---
title: agreementFile 资源类型
description: 表示租户使用 Azure Active Directory 和 Azure AD (管理的可自定义) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: fde0912f767510c0c5cd1bf984354099b37be9b0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722617"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="604a3-103">agreementFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="604a3-103">agreementFile resource type</span></span>

<span data-ttu-id="604a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="604a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="604a3-105">表示租户使用 Azure Active Directory 和 Azure AD (管理的可自定义) 。</span><span class="sxs-lookup"><span data-stu-id="604a3-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="604a3-106">它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。</span><span class="sxs-lookup"><span data-stu-id="604a3-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="604a3-107">属性</span><span class="sxs-lookup"><span data-stu-id="604a3-107">Properties</span></span>
| <span data-ttu-id="604a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="604a3-108">Property</span></span>     | <span data-ttu-id="604a3-109">类型</span><span class="sxs-lookup"><span data-stu-id="604a3-109">Type</span></span>        | <span data-ttu-id="604a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="604a3-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="604a3-111">fileData</span><span class="sxs-lookup"><span data-stu-id="604a3-111">fileData</span></span>|[<span data-ttu-id="604a3-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="604a3-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="604a3-113">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="604a3-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="604a3-114">只读。</span><span class="sxs-lookup"><span data-stu-id="604a3-114">Read-only.</span></span>|
|<span data-ttu-id="604a3-115">fileName</span><span class="sxs-lookup"><span data-stu-id="604a3-115">fileName</span></span>|<span data-ttu-id="604a3-116">String</span><span class="sxs-lookup"><span data-stu-id="604a3-116">String</span></span>|<span data-ttu-id="604a3-117">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="604a3-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="604a3-118">只读。</span><span class="sxs-lookup"><span data-stu-id="604a3-118">Read-only.</span></span>|
|<span data-ttu-id="604a3-119">id</span><span class="sxs-lookup"><span data-stu-id="604a3-119">id</span></span>|<span data-ttu-id="604a3-120">字符串</span><span class="sxs-lookup"><span data-stu-id="604a3-120">String</span></span>|<span data-ttu-id="604a3-121">协议文件的标识符。</span><span class="sxs-lookup"><span data-stu-id="604a3-121">The identifier of the agreement file.</span></span> <span data-ttu-id="604a3-122">只读。</span><span class="sxs-lookup"><span data-stu-id="604a3-122">Read-only.</span></span>|
|<span data-ttu-id="604a3-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="604a3-123">isDefault</span></span>|<span data-ttu-id="604a3-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="604a3-124">Boolean</span></span>|<span data-ttu-id="604a3-125">如果没有任何语言与客户端首选项匹配，则指示这是默认协议文件。</span><span class="sxs-lookup"><span data-stu-id="604a3-125">If none of the languages matches the client preference, indicates that this is the default agreement file.</span></span> <span data-ttu-id="604a3-126">如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。</span><span class="sxs-lookup"><span data-stu-id="604a3-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="604a3-127">只读。</span><span class="sxs-lookup"><span data-stu-id="604a3-127">Read-only.</span></span>|
|<span data-ttu-id="604a3-128">language</span><span class="sxs-lookup"><span data-stu-id="604a3-128">language</span></span>|<span data-ttu-id="604a3-129">String</span><span class="sxs-lookup"><span data-stu-id="604a3-129">String</span></span>|<span data-ttu-id="604a3-130">协议文件的语言，格式为 languagecode2-country/regioncode2。</span><span class="sxs-lookup"><span data-stu-id="604a3-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="604a3-131">languagecode2 是从 ISO 639-1 派生的两个字母小写代码。</span><span class="sxs-lookup"><span data-stu-id="604a3-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="604a3-132">country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。</span><span class="sxs-lookup"><span data-stu-id="604a3-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="604a3-133">只读。</span><span class="sxs-lookup"><span data-stu-id="604a3-133">Read-only.</span></span>|
|<span data-ttu-id="604a3-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="604a3-134">isMajorVersion</span></span>|<span data-ttu-id="604a3-135">布尔值</span><span class="sxs-lookup"><span data-stu-id="604a3-135">Boolean</span></span>|<span data-ttu-id="604a3-136">指示协议文件是否是主要版本更新。</span><span class="sxs-lookup"><span data-stu-id="604a3-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="604a3-137">主要版本更新使协议在相应语言的接受无效。</span><span class="sxs-lookup"><span data-stu-id="604a3-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="604a3-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="604a3-138">createdDateTime</span></span>|<span data-ttu-id="604a3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="604a3-139">DateTimeOffset</span></span>|<span data-ttu-id="604a3-140">表示文件创建时间的日期时间。</span><span class="sxs-lookup"><span data-stu-id="604a3-140">The date time representing when the file was created.</span></span> <span data-ttu-id="604a3-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="604a3-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="604a3-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="604a3-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|

<!--
## Relationships
| Relationship | Type        | Description |
|:-------------|:------------|:------------|
|localizations|[agreementFileLocalization](agreementfilelocalization.md) collection|The localized version of the agreement files attached to the agreement.|
-->

## <a name="json-representation"></a><span data-ttu-id="604a3-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="604a3-143">JSON representation</span></span>

<span data-ttu-id="604a3-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="604a3-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.agreementFile",
  "keyProperty": "id"
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


