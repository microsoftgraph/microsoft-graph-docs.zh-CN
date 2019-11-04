---
title: itemPhone 资源类型
description: itemPhone 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a40a0a096fa6f0616a8ff44e41e25791873fa82f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939318"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="1adfc-103">itemPhone 资源类型</span><span class="sxs-lookup"><span data-stu-id="1adfc-103">itemPhone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1adfc-104">表示有关用户在各种服务中关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1adfc-104">Represents detailed information about phone numbers the user has associated in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="1adfc-105">方法</span><span class="sxs-lookup"><span data-stu-id="1adfc-105">Methods</span></span>

| <span data-ttu-id="1adfc-106">方法</span><span class="sxs-lookup"><span data-stu-id="1adfc-106">Method</span></span>                                     | <span data-ttu-id="1adfc-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="1adfc-107">Return Type</span></span>               | <span data-ttu-id="1adfc-108">说明</span><span class="sxs-lookup"><span data-stu-id="1adfc-108">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="1adfc-109">获取 itemPhone</span><span class="sxs-lookup"><span data-stu-id="1adfc-109">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="1adfc-110">itemPhone</span><span class="sxs-lookup"><span data-stu-id="1adfc-110">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="1adfc-111">读取**itemPhone**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1adfc-111">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="1adfc-112">更新 itemPhone</span><span class="sxs-lookup"><span data-stu-id="1adfc-112">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="1adfc-113">itemPhone</span><span class="sxs-lookup"><span data-stu-id="1adfc-113">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="1adfc-114">更新**itemPhone**对象。</span><span class="sxs-lookup"><span data-stu-id="1adfc-114">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="1adfc-115">删除 itemPhone</span><span class="sxs-lookup"><span data-stu-id="1adfc-115">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="1adfc-116">无</span><span class="sxs-lookup"><span data-stu-id="1adfc-116">None</span></span>                      | <span data-ttu-id="1adfc-117">删除**itemPhone**对象。</span><span class="sxs-lookup"><span data-stu-id="1adfc-117">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="1adfc-118">属性</span><span class="sxs-lookup"><span data-stu-id="1adfc-118">Properties</span></span>

| <span data-ttu-id="1adfc-119">属性</span><span class="sxs-lookup"><span data-stu-id="1adfc-119">Property</span></span>     | <span data-ttu-id="1adfc-120">类型</span><span class="sxs-lookup"><span data-stu-id="1adfc-120">Type</span></span>        | <span data-ttu-id="1adfc-121">说明</span><span class="sxs-lookup"><span data-stu-id="1adfc-121">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="1adfc-122">displayName</span><span class="sxs-lookup"><span data-stu-id="1adfc-122">displayName</span></span>   |<span data-ttu-id="1adfc-123">字符串</span><span class="sxs-lookup"><span data-stu-id="1adfc-123">String</span></span>       | <span data-ttu-id="1adfc-124">包含电话号码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="1adfc-124">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="1adfc-125">number</span><span class="sxs-lookup"><span data-stu-id="1adfc-125">number</span></span>        |<span data-ttu-id="1adfc-126">字符串</span><span class="sxs-lookup"><span data-stu-id="1adfc-126">String</span></span>       | <span data-ttu-id="1adfc-127">包含电话号码。</span><span class="sxs-lookup"><span data-stu-id="1adfc-127">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="1adfc-128">类型</span><span class="sxs-lookup"><span data-stu-id="1adfc-128">type</span></span>          |<span data-ttu-id="1adfc-129">字符串</span><span class="sxs-lookup"><span data-stu-id="1adfc-129">string</span></span>       | <span data-ttu-id="1adfc-130">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="1adfc-130">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1adfc-131">关系</span><span class="sxs-lookup"><span data-stu-id="1adfc-131">Relationships</span></span>

<span data-ttu-id="1adfc-132">无</span><span class="sxs-lookup"><span data-stu-id="1adfc-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1adfc-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1adfc-133">JSON representation</span></span>

<span data-ttu-id="1adfc-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1adfc-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "number": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemPhone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
