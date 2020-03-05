---
title: languageProficiency 资源类型
description: languageProficiency 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0934ea66c15e090a4f9ba9bcaa62a6c7eb900cd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522993"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="b7140-103">languageProficiency 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7140-103">languageProficiency resource type</span></span>

<span data-ttu-id="b7140-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b7140-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7140-105">表示有关用户已添加到其[配置文件](profile.md)中的语言的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b7140-105">Represents detailed information about languages that a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="b7140-106">继承自[itemFacet](itemFacet.md)。</span><span class="sxs-lookup"><span data-stu-id="b7140-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b7140-107">方法</span><span class="sxs-lookup"><span data-stu-id="b7140-107">Methods</span></span>

| <span data-ttu-id="b7140-108">方法</span><span class="sxs-lookup"><span data-stu-id="b7140-108">Method</span></span>                                                       | <span data-ttu-id="b7140-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b7140-109">Return Type</span></span>                                   | <span data-ttu-id="b7140-110">说明</span><span class="sxs-lookup"><span data-stu-id="b7140-110">Description</span></span>                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="b7140-111">获取 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="b7140-111">Get languageProficiency</span></span>](../api/languageproficiency-get.md) | [<span data-ttu-id="b7140-112">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="b7140-112">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="b7140-113">读取**languageProficiency**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7140-113">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="b7140-114">更新 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="b7140-114">Update languageProficiency</span></span>](../api/languageproficiency-update.md)               | [<span data-ttu-id="b7140-115">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="b7140-115">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="b7140-116">更新**languageProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="b7140-116">Update a **languageProficiency** object.</span></span>                               |
| [<span data-ttu-id="b7140-117">删除 languageProficiency</span><span class="sxs-lookup"><span data-stu-id="b7140-117">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)               | <span data-ttu-id="b7140-118">无</span><span class="sxs-lookup"><span data-stu-id="b7140-118">None</span></span>                                          | <span data-ttu-id="b7140-119">删除**languageProficiency**对象。</span><span class="sxs-lookup"><span data-stu-id="b7140-119">Delete a **languageProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="b7140-120">属性</span><span class="sxs-lookup"><span data-stu-id="b7140-120">Properties</span></span>

| <span data-ttu-id="b7140-121">属性</span><span class="sxs-lookup"><span data-stu-id="b7140-121">Property</span></span>     | <span data-ttu-id="b7140-122">类型</span><span class="sxs-lookup"><span data-stu-id="b7140-122">Type</span></span>        | <span data-ttu-id="b7140-123">说明</span><span class="sxs-lookup"><span data-stu-id="b7140-123">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b7140-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b7140-124">displayName</span></span>   |<span data-ttu-id="b7140-125">String</span><span class="sxs-lookup"><span data-stu-id="b7140-125">String</span></span>       | <span data-ttu-id="b7140-126">包含语言的长格式名称。</span><span class="sxs-lookup"><span data-stu-id="b7140-126">Contains the long-form name for the language.</span></span>                                                                                                   |
|<span data-ttu-id="b7140-127">水平</span><span class="sxs-lookup"><span data-stu-id="b7140-127">proficiency</span></span>   |<span data-ttu-id="b7140-128">string</span><span class="sxs-lookup"><span data-stu-id="b7140-128">string</span></span>       | <span data-ttu-id="b7140-129">可取值为：`elementary`、`conversational`、`limitedWorking`、`professionalWorking`、`fullProfessional`、`nativeOrBilingual` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b7140-129">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b7140-130">tag</span><span class="sxs-lookup"><span data-stu-id="b7140-130">tag</span></span>           |<span data-ttu-id="b7140-131">String</span><span class="sxs-lookup"><span data-stu-id="b7140-131">String</span></span>       | <span data-ttu-id="b7140-132">包含四个字符的语言的 BCP47 名称（en-us，无 NB，en-us）。</span><span class="sxs-lookup"><span data-stu-id="b7140-132">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                                  |

## <a name="relationships"></a><span data-ttu-id="b7140-133">关系</span><span class="sxs-lookup"><span data-stu-id="b7140-133">Relationships</span></span>

<span data-ttu-id="b7140-134">无。</span><span class="sxs-lookup"><span data-stu-id="b7140-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7140-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7140-135">JSON representation</span></span>

<span data-ttu-id="b7140-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7140-136">The following is a JSON representation of the resource.</span></span> 

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
