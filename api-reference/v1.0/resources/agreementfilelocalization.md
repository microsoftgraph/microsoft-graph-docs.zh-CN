---
title: agreementFileLocalization 资源类型
description: 表示 Azure Active Directory (Azure AD) 中的使用条款的本地化策略文件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 85d5730dda21bec937044d61db0e46dc3473728e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761882"
---
# <a name="agreementfilelocalization-resource-type"></a><span data-ttu-id="2a6d2-103">agreementFileLocalization 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a6d2-103">agreementFileLocalization resource type</span></span>

<span data-ttu-id="2a6d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a6d2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a6d2-105">表示租户使用 Azure Active Directory 和 Azure AD (管理的可自定义) 。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="2a6d2-106">它包含有关协议文件的元数据 (例如，名称、语言以及它是否是协议文件的默认) 。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

## <a name="properties"></a><span data-ttu-id="2a6d2-107">属性</span><span class="sxs-lookup"><span data-stu-id="2a6d2-107">Properties</span></span>
| <span data-ttu-id="2a6d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a6d2-108">Property</span></span>     | <span data-ttu-id="2a6d2-109">类型</span><span class="sxs-lookup"><span data-stu-id="2a6d2-109">Type</span></span>        | <span data-ttu-id="2a6d2-110">说明</span><span class="sxs-lookup"><span data-stu-id="2a6d2-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2a6d2-111">fileData</span><span class="sxs-lookup"><span data-stu-id="2a6d2-111">fileData</span></span>|[<span data-ttu-id="2a6d2-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="2a6d2-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="2a6d2-113">表示 PDF 文档的使用条款的数据。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-113">Data that represents the terms of use PDF document.</span></span> <span data-ttu-id="2a6d2-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-114">Read-only.</span></span>|
|<span data-ttu-id="2a6d2-115">fileName</span><span class="sxs-lookup"><span data-stu-id="2a6d2-115">fileName</span></span>|<span data-ttu-id="2a6d2-116">String</span><span class="sxs-lookup"><span data-stu-id="2a6d2-116">String</span></span>|<span data-ttu-id="2a6d2-117">协议文件的名称 (例如，TOU.pdf) 。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="2a6d2-118">只读。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-118">Read-only.</span></span>|
|<span data-ttu-id="2a6d2-119">id</span><span class="sxs-lookup"><span data-stu-id="2a6d2-119">id</span></span>|<span data-ttu-id="2a6d2-120">字符串</span><span class="sxs-lookup"><span data-stu-id="2a6d2-120">String</span></span>|<span data-ttu-id="2a6d2-121">agreementFileLocalization 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-121">The identifier of the agreementFileLocalization object.</span></span> <span data-ttu-id="2a6d2-122">只读。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-122">Read-only.</span></span>|
|<span data-ttu-id="2a6d2-123">isDefault</span><span class="sxs-lookup"><span data-stu-id="2a6d2-123">isDefault</span></span>|<span data-ttu-id="2a6d2-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a6d2-124">Boolean</span></span>| <span data-ttu-id="2a6d2-125">如果没有任何语言与客户端首选项匹配，则指示这是默认协议文件。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-125">If none of the languages matches the client preference, indicates that this is the default agreement file.</span></span> <span data-ttu-id="2a6d2-126">如果未将任何文件标记为默认文件，则第一个文件将被视为默认文件。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-126">If none of the files are marked as default, the first one is treated as the default.</span></span> <span data-ttu-id="2a6d2-127">只读。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-127">Read-only.</span></span>|
|<span data-ttu-id="2a6d2-128">language</span><span class="sxs-lookup"><span data-stu-id="2a6d2-128">language</span></span>|<span data-ttu-id="2a6d2-129">String</span><span class="sxs-lookup"><span data-stu-id="2a6d2-129">String</span></span>|<span data-ttu-id="2a6d2-130">协议文件的语言，格式为 languagecode2-country/regioncode2。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-130">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="2a6d2-131">languagecode2 是从 ISO 639-1 派生的两个字母小写代码。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-131">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="2a6d2-132">country/regioncode2 派生自 ISO 3166，通常由两个小写字母或 BCP-47 语言标记 (例如 en-US) 。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-132">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="2a6d2-133">只读。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-133">Read-only.</span></span>|
|<span data-ttu-id="2a6d2-134">isMajorVersion</span><span class="sxs-lookup"><span data-stu-id="2a6d2-134">isMajorVersion</span></span>|<span data-ttu-id="2a6d2-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a6d2-135">Boolean</span></span>|<span data-ttu-id="2a6d2-136">指示协议文件是否是主要版本更新。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-136">Indicates whether the agreement file is a major version update.</span></span> <span data-ttu-id="2a6d2-137">主要版本更新使协议在相应语言的接受无效。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-137">Major version updates invalidate the agreement's acceptances on the corresponding language.</span></span> |
|<span data-ttu-id="2a6d2-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a6d2-138">createdDateTime</span></span>|<span data-ttu-id="2a6d2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a6d2-139">DateTimeOffset</span></span>|<span data-ttu-id="2a6d2-140">表示文件创建时间的日期时间。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-140">The date time representing when the file was created.</span></span> <span data-ttu-id="2a6d2-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2a6d2-142">例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-142">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span>|
|<span data-ttu-id="2a6d2-143">displayName</span><span class="sxs-lookup"><span data-stu-id="2a6d2-143">displayName</span></span>|<span data-ttu-id="2a6d2-144">字符串</span><span class="sxs-lookup"><span data-stu-id="2a6d2-144">String</span></span>|<span data-ttu-id="2a6d2-145">协议的显示名称文件的本地化版本。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-145">Localized display name of the policy file of an agreement.</span></span> <span data-ttu-id="2a6d2-146">本地化显示名称向查看协议的最终用户显示。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-146">The localized display name is shown to end users who view the agreement.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a6d2-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a6d2-147">JSON representation</span></span>

<span data-ttu-id="2a6d2-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a6d2-148">The following is a JSON representation of the resource.</span></span>

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
