---
title: agreementFile 资源类型
description: 表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。 它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511427"
---
# <a name="agreementfile-resource-type"></a><span data-ttu-id="b4be2-104">agreementFile 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4be2-104">agreementFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4be2-105">表示使用协议文件租户管理使用 Azure Active Directory (Azure AD) 的可自定义术语。</span><span class="sxs-lookup"><span data-stu-id="b4be2-105">Represents a customizable terms of use agreement file that a tenant manages with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="b4be2-106">它包含有关协议文件的元数据 (例如，名称、 语言，以及它是否为默认的文件)。</span><span class="sxs-lookup"><span data-stu-id="b4be2-106">It contains metadata about the agreement file (for example, the name, the language, and whether it is the default file).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a><span data-ttu-id="b4be2-107">属性</span><span class="sxs-lookup"><span data-stu-id="b4be2-107">Properties</span></span>
| <span data-ttu-id="b4be2-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4be2-108">Property</span></span>     | <span data-ttu-id="b4be2-109">类型</span><span class="sxs-lookup"><span data-stu-id="b4be2-109">Type</span></span>        | <span data-ttu-id="b4be2-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4be2-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4be2-111">fileData</span><span class="sxs-lookup"><span data-stu-id="b4be2-111">fileData</span></span>|[<span data-ttu-id="b4be2-112">agreementFileData</span><span class="sxs-lookup"><span data-stu-id="b4be2-112">agreementFileData</span></span>](agreementfiledata.md)|<span data-ttu-id="b4be2-113">表示使用 PDF 文档中的条款的数据。</span><span class="sxs-lookup"><span data-stu-id="b4be2-113">Data representing the terms of use PDF document.</span></span> <span data-ttu-id="b4be2-114">只读。</span><span class="sxs-lookup"><span data-stu-id="b4be2-114">Read-only.</span></span>|
|<span data-ttu-id="b4be2-115">fileName</span><span class="sxs-lookup"><span data-stu-id="b4be2-115">fileName</span></span>|<span data-ttu-id="b4be2-116">String</span><span class="sxs-lookup"><span data-stu-id="b4be2-116">String</span></span>|<span data-ttu-id="b4be2-117">协议文件 (例如，TOU.pdf) 的名称。</span><span class="sxs-lookup"><span data-stu-id="b4be2-117">Name of the agreement file (for example, TOU.pdf).</span></span> <span data-ttu-id="b4be2-118">只读。</span><span class="sxs-lookup"><span data-stu-id="b4be2-118">Read-only.</span></span>|
|<span data-ttu-id="b4be2-119">id</span><span class="sxs-lookup"><span data-stu-id="b4be2-119">id</span></span>|<span data-ttu-id="b4be2-120">String</span><span class="sxs-lookup"><span data-stu-id="b4be2-120">String</span></span>|<span data-ttu-id="b4be2-121">只读。</span><span class="sxs-lookup"><span data-stu-id="b4be2-121">Read-only.</span></span>|
|<span data-ttu-id="b4be2-122">isDefault</span><span class="sxs-lookup"><span data-stu-id="b4be2-122">isDefault</span></span>|<span data-ttu-id="b4be2-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4be2-123">Boolean</span></span>|<span data-ttu-id="b4be2-124">指示是否这是默认协议文件，是否无区域性匹配的客户端首选项。</span><span class="sxs-lookup"><span data-stu-id="b4be2-124">Indicates whether this is the default agreement file if none of the cultures matches the client preference.</span></span> <span data-ttu-id="b4be2-125">如果没有任何文件被标记为默认值，第一个将被视为默认值。</span><span class="sxs-lookup"><span data-stu-id="b4be2-125">If none of the files are marked as default, the first one will be treated as the default.</span></span> <span data-ttu-id="b4be2-126">只读。</span><span class="sxs-lookup"><span data-stu-id="b4be2-126">Read-only.</span></span>|
|<span data-ttu-id="b4be2-127">language</span><span class="sxs-lookup"><span data-stu-id="b4be2-127">language</span></span>|<span data-ttu-id="b4be2-128">String</span><span class="sxs-lookup"><span data-stu-id="b4be2-128">String</span></span>|<span data-ttu-id="b4be2-129">区域性格式 languagecode2-国家/地区/regioncode2 中的协议文件。</span><span class="sxs-lookup"><span data-stu-id="b4be2-129">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="b4be2-130">languagecode2 是小写字母双字母代码派生自 ISO 639-1。</span><span class="sxs-lookup"><span data-stu-id="b4be2-130">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="b4be2-131">国家/地区/regioncode2 派生自 ISO 3166，它通常包括两个大写字母或 BCP 47 语言标记 (例如，EN-US)。</span><span class="sxs-lookup"><span data-stu-id="b4be2-131">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span> <span data-ttu-id="b4be2-132">只读。</span><span class="sxs-lookup"><span data-stu-id="b4be2-132">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4be2-133">关系</span><span class="sxs-lookup"><span data-stu-id="b4be2-133">Relationships</span></span>
<span data-ttu-id="b4be2-134">无。</span><span class="sxs-lookup"><span data-stu-id="b4be2-134">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b4be2-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4be2-135">JSON representation</span></span>

<span data-ttu-id="b4be2-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4be2-136">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
