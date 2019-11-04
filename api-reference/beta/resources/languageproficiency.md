---
title: languageProficiency 资源类型
description: languageProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4e2ea70eca4e830ef334e5bf61be724cb05f1cfc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939290"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="027e3-103">languageProficiency 资源类型</span><span class="sxs-lookup"><span data-stu-id="027e3-103">languageProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="027e3-104">表示有关用户已添加到其[配置文件](profile.md)中的语言的详细信息。</span><span class="sxs-lookup"><span data-stu-id="027e3-104">Represents detailed information about a languages a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="027e3-105">继承自[itemFacet](itemFacet.md)。</span><span class="sxs-lookup"><span data-stu-id="027e3-105">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="027e3-106">方法</span><span class="sxs-lookup"><span data-stu-id="027e3-106">Methods</span></span>

| <span data-ttu-id="027e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="027e3-107">Method</span></span>                                                       | <span data-ttu-id="027e3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="027e3-108">Return Type</span></span>                                   | <span data-ttu-id="027e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="027e3-109">Description</span></span>                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="027e3-110">获取 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="027e3-110">Get languageProficiency</span></span>](../api/languageproficiency-get.md) | [<span data-ttu-id="027e3-111">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="027e3-111">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="027e3-112">读取**languageProficiency**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="027e3-112">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="027e3-113">更新 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="027e3-113">Update languageProficiency</span></span>](../api/languageproficiency-update.md)               | [<span data-ttu-id="027e3-114">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="027e3-114">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="027e3-115">更新**languageProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="027e3-115">Update a **languageProficiency** object.</span></span>                               |
| [<span data-ttu-id="027e3-116">删除 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="027e3-116">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)               | <span data-ttu-id="027e3-117">无</span><span class="sxs-lookup"><span data-stu-id="027e3-117">None</span></span>                                          | <span data-ttu-id="027e3-118">删除**languageProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="027e3-118">Delete a **languageProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="027e3-119">属性</span><span class="sxs-lookup"><span data-stu-id="027e3-119">Properties</span></span>

| <span data-ttu-id="027e3-120">属性</span><span class="sxs-lookup"><span data-stu-id="027e3-120">Property</span></span>     | <span data-ttu-id="027e3-121">类型</span><span class="sxs-lookup"><span data-stu-id="027e3-121">Type</span></span>        | <span data-ttu-id="027e3-122">说明</span><span class="sxs-lookup"><span data-stu-id="027e3-122">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="027e3-123">displayName</span><span class="sxs-lookup"><span data-stu-id="027e3-123">displayName</span></span>   |<span data-ttu-id="027e3-124">String</span><span class="sxs-lookup"><span data-stu-id="027e3-124">String</span></span>       | <span data-ttu-id="027e3-125">包含语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="027e3-125">Contains the long-form name for the language.</span></span>                                                                                                   |
|<span data-ttu-id="027e3-126">水平</span><span class="sxs-lookup"><span data-stu-id="027e3-126">proficiency</span></span>   |<span data-ttu-id="027e3-127">string</span><span class="sxs-lookup"><span data-stu-id="027e3-127">string</span></span>       | <span data-ttu-id="027e3-128">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="027e3-128">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="027e3-129">tag</span><span class="sxs-lookup"><span data-stu-id="027e3-129">tag</span></span>           |<span data-ttu-id="027e3-130">字符串</span><span class="sxs-lookup"><span data-stu-id="027e3-130">String</span></span>       | <span data-ttu-id="027e3-131">包含四个字符的语言的 BCP47 名称（en-us，无 NB，en-us）。</span><span class="sxs-lookup"><span data-stu-id="027e3-131">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                                  |

## <a name="relationships"></a><span data-ttu-id="027e3-132">关系</span><span class="sxs-lookup"><span data-stu-id="027e3-132">Relationships</span></span>

<span data-ttu-id="027e3-133">无</span><span class="sxs-lookup"><span data-stu-id="027e3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="027e3-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="027e3-134">JSON representation</span></span>

<span data-ttu-id="027e3-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="027e3-135">The following is a JSON representation of the resource.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "proficiency": "string",
  "tag": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "languageProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
