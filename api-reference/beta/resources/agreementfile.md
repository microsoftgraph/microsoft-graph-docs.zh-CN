---
title: agreementFile 资源类型
description: 表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。 它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。
localization_priority: Normal
ms.openlocfilehash: f06792d63deabf25659a09e8aec5ed0e8f036472
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804506"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="39e6e-104">agreementFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="39e6e-104">agreementFile resource type</span></span>

> <span data-ttu-id="39e6e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="39e6e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39e6e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="39e6e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="39e6e-107">表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。</span><span class="sxs-lookup"><span data-stu-id="39e6e-107">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="39e6e-108">它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。</span><span class="sxs-lookup"><span data-stu-id="39e6e-108">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="39e6e-109">属性</span><span class="sxs-lookup"><span data-stu-id="39e6e-109">Properties</span></span>
| <span data-ttu-id="39e6e-110">属性</span><span class="sxs-lookup"><span data-stu-id="39e6e-110">Property</span></span>     | <span data-ttu-id="39e6e-111">类型</span><span class="sxs-lookup"><span data-stu-id="39e6e-111">Type</span></span>        | <span data-ttu-id="39e6e-112">Description</span><span class="sxs-lookup"><span data-stu-id="39e6e-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39e6e-113">fileData</span><span class="sxs-lookup"><span data-stu-id="39e6e-113">fileData</span></span>|[<span data-ttu-id="39e6e-114">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="39e6e-114">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="39e6e-115">表示使用 PDF 文档中的条款的数据。</span><span class="sxs-lookup"><span data-stu-id="39e6e-115">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="39e6e-116">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="39e6e-116">Read-only.</span></span>|
|<span data-ttu-id="39e6e-117">fileName</span><span class="sxs-lookup"><span data-stu-id="39e6e-117">fileName</span></span>|<span data-ttu-id="39e6e-118">String</span><span class="sxs-lookup"><span data-stu-id="39e6e-118">String</span></span>|<span data-ttu-id="39e6e-119">协议文件 (例如，TOU.pdf) 的名称。</span><span class="sxs-lookup"><span data-stu-id="39e6e-119">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="39e6e-120">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="39e6e-120">Read-only.</span></span>|
|<span data-ttu-id="39e6e-121">id</span><span class="sxs-lookup"><span data-stu-id="39e6e-121">id</span></span>|<span data-ttu-id="39e6e-122">String</span><span class="sxs-lookup"><span data-stu-id="39e6e-122">String</span></span>|<span data-ttu-id="39e6e-123">只读。</span><span class="sxs-lookup"><span data-stu-id="39e6e-123">Read-only.</span></span>|
|<span data-ttu-id="39e6e-124">isDefault</span><span class="sxs-lookup"><span data-stu-id="39e6e-124">isDefault</span></span>|<span data-ttu-id="39e6e-125">布尔</span><span class="sxs-lookup"><span data-stu-id="39e6e-125">Boolean</span></span>|<span data-ttu-id="39e6e-126">指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。</span><span class="sxs-lookup"><span data-stu-id="39e6e-126">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="39e6e-127">如果没有任何文件被标记为默认值，第一个将被视为默认值。</span><span class="sxs-lookup"><span data-stu-id="39e6e-127">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="39e6e-128">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="39e6e-128">Read-only.</span></span>|
|<span data-ttu-id="39e6e-129">language</span><span class="sxs-lookup"><span data-stu-id="39e6e-129">language</span></span>|<span data-ttu-id="39e6e-130">String</span><span class="sxs-lookup"><span data-stu-id="39e6e-130">String</span></span>|<span data-ttu-id="39e6e-131">区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。</span><span class="sxs-lookup"><span data-stu-id="39e6e-131">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="39e6e-132">languagecode2 是小写字母双字母代码派生自 ISO 639-1。</span><span class="sxs-lookup"><span data-stu-id="39e6e-132">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="39e6e-133">国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。</span><span class="sxs-lookup"><span data-stu-id="39e6e-133">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="39e6e-134">只读。</span><span class="sxs-lookup"><span data-stu-id="39e6e-134">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39e6e-135">Relationships</span><span class="sxs-lookup"><span data-stu-id="39e6e-135">Relationships</span></span>
<span data-ttu-id="39e6e-136">无。</span><span class="sxs-lookup"><span data-stu-id="39e6e-136">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="39e6e-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39e6e-137">JSON representation</span></span>

<span data-ttu-id="39e6e-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39e6e-138">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
