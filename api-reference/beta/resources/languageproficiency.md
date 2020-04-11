---
title: languageProficiency 资源类型
description: languageProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48a9e26bde5d06b834c542cbb987a2faff9fc23c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229393"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="d059f-103">languageProficiency 资源类型</span><span class="sxs-lookup"><span data-stu-id="d059f-103">languageProficiency resource type</span></span>

<span data-ttu-id="d059f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d059f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d059f-105">表示有关用户已添加到其[配置文件](profile.md)中的语言的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d059f-105">Represents detailed information about languages that a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="d059f-106">继承自[itemFacet](itemFacet.md)。</span><span class="sxs-lookup"><span data-stu-id="d059f-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d059f-107">方法</span><span class="sxs-lookup"><span data-stu-id="d059f-107">Methods</span></span>

| <span data-ttu-id="d059f-108">方法</span><span class="sxs-lookup"><span data-stu-id="d059f-108">Method</span></span>                                                              | <span data-ttu-id="d059f-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d059f-109">Return Type</span></span>                                   | <span data-ttu-id="d059f-110">说明</span><span class="sxs-lookup"><span data-stu-id="d059f-110">Description</span></span>                                                                |
|:--------------------------------------------------------------------|:----------------------------------------------|:---------------------------------------------------------------------------|
| [<span data-ttu-id="d059f-111">获取 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="d059f-111">Get languageProficiency</span></span>](../api/languageproficiency-get.md)        | [<span data-ttu-id="d059f-112">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="d059f-112">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="d059f-113">读取**languageProficiency**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d059f-113">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="d059f-114">更新 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="d059f-114">Update languageProficiency</span></span>](../api/languageproficiency-update.md)  | [<span data-ttu-id="d059f-115">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="d059f-115">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="d059f-116">更新**languageProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="d059f-116">Update a **languageProficiency** object.</span></span>                                   |
| [<span data-ttu-id="d059f-117">删除 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="d059f-117">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)  | <span data-ttu-id="d059f-118">无</span><span class="sxs-lookup"><span data-stu-id="d059f-118">None</span></span>                                          | <span data-ttu-id="d059f-119">删除**languageProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="d059f-119">Delete a **languageProficiency** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="d059f-120">属性</span><span class="sxs-lookup"><span data-stu-id="d059f-120">Properties</span></span>

| <span data-ttu-id="d059f-121">属性</span><span class="sxs-lookup"><span data-stu-id="d059f-121">Property</span></span>     | <span data-ttu-id="d059f-122">类型</span><span class="sxs-lookup"><span data-stu-id="d059f-122">Type</span></span>        | <span data-ttu-id="d059f-123">说明</span><span class="sxs-lookup"><span data-stu-id="d059f-123">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d059f-124">displayName</span><span class="sxs-lookup"><span data-stu-id="d059f-124">displayName</span></span>   |<span data-ttu-id="d059f-125">String</span><span class="sxs-lookup"><span data-stu-id="d059f-125">String</span></span>       | <span data-ttu-id="d059f-126">包含语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="d059f-126">Contains the long-form name for the language.</span></span>                                                                                                               |
|<span data-ttu-id="d059f-127">水平</span><span class="sxs-lookup"><span data-stu-id="d059f-127">proficiency</span></span>   |<span data-ttu-id="d059f-128">string</span><span class="sxs-lookup"><span data-stu-id="d059f-128">string</span></span>       | <span data-ttu-id="d059f-129">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d059f-129">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="d059f-130">tag</span><span class="sxs-lookup"><span data-stu-id="d059f-130">tag</span></span>           |<span data-ttu-id="d059f-131">String</span><span class="sxs-lookup"><span data-stu-id="d059f-131">String</span></span>       | <span data-ttu-id="d059f-132">包含四个字符的语言的 BCP47 名称（en-us，无 NB，en-us）。</span><span class="sxs-lookup"><span data-stu-id="d059f-132">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                              |

## <a name="relationships"></a><span data-ttu-id="d059f-133">关系</span><span class="sxs-lookup"><span data-stu-id="d059f-133">Relationships</span></span>

<span data-ttu-id="d059f-134">无。</span><span class="sxs-lookup"><span data-stu-id="d059f-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d059f-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d059f-135">JSON representation</span></span>

<span data-ttu-id="d059f-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d059f-136">The following is a JSON representation of the resource.</span></span>

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
