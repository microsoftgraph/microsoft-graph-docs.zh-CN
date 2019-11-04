---
title: itemPhone 资源类型
description: itemPhone 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2ba1fce4492bfacb3a44f21a0fc55ddd8d37b068
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950435"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="dab7d-103">itemPhone 资源类型</span><span class="sxs-lookup"><span data-stu-id="dab7d-103">itemPhone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dab7d-104">表示有关与各种服务中的用户关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="dab7d-104">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="dab7d-105">方法</span><span class="sxs-lookup"><span data-stu-id="dab7d-105">Methods</span></span>

| <span data-ttu-id="dab7d-106">方法</span><span class="sxs-lookup"><span data-stu-id="dab7d-106">Method</span></span>                                     | <span data-ttu-id="dab7d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="dab7d-107">Return Type</span></span>               | <span data-ttu-id="dab7d-108">说明</span><span class="sxs-lookup"><span data-stu-id="dab7d-108">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="dab7d-109">获取 itemPhone</span><span class="sxs-lookup"><span data-stu-id="dab7d-109">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="dab7d-110">itemPhone</span><span class="sxs-lookup"><span data-stu-id="dab7d-110">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="dab7d-111">读取**itemPhone**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dab7d-111">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="dab7d-112">更新 itemPhone</span><span class="sxs-lookup"><span data-stu-id="dab7d-112">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="dab7d-113">itemPhone</span><span class="sxs-lookup"><span data-stu-id="dab7d-113">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="dab7d-114">更新**itemPhone**对象。</span><span class="sxs-lookup"><span data-stu-id="dab7d-114">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="dab7d-115">删除 itemPhone</span><span class="sxs-lookup"><span data-stu-id="dab7d-115">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="dab7d-116">无</span><span class="sxs-lookup"><span data-stu-id="dab7d-116">None</span></span>                      | <span data-ttu-id="dab7d-117">删除**itemPhone**对象。</span><span class="sxs-lookup"><span data-stu-id="dab7d-117">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="dab7d-118">属性</span><span class="sxs-lookup"><span data-stu-id="dab7d-118">Properties</span></span>

| <span data-ttu-id="dab7d-119">属性</span><span class="sxs-lookup"><span data-stu-id="dab7d-119">Property</span></span>     | <span data-ttu-id="dab7d-120">类型</span><span class="sxs-lookup"><span data-stu-id="dab7d-120">Type</span></span>        | <span data-ttu-id="dab7d-121">说明</span><span class="sxs-lookup"><span data-stu-id="dab7d-121">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="dab7d-122">displayName</span><span class="sxs-lookup"><span data-stu-id="dab7d-122">displayName</span></span>   |<span data-ttu-id="dab7d-123">String</span><span class="sxs-lookup"><span data-stu-id="dab7d-123">String</span></span>       | <span data-ttu-id="dab7d-124">包含电话号码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="dab7d-124">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="dab7d-125">number</span><span class="sxs-lookup"><span data-stu-id="dab7d-125">number</span></span>        |<span data-ttu-id="dab7d-126">String</span><span class="sxs-lookup"><span data-stu-id="dab7d-126">String</span></span>       | <span data-ttu-id="dab7d-127">包含电话号码。</span><span class="sxs-lookup"><span data-stu-id="dab7d-127">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="dab7d-128">类型</span><span class="sxs-lookup"><span data-stu-id="dab7d-128">type</span></span>          |<span data-ttu-id="dab7d-129">字符串</span><span class="sxs-lookup"><span data-stu-id="dab7d-129">string</span></span>       | <span data-ttu-id="dab7d-130">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="dab7d-130">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dab7d-131">关系</span><span class="sxs-lookup"><span data-stu-id="dab7d-131">Relationships</span></span>

<span data-ttu-id="dab7d-132">无</span><span class="sxs-lookup"><span data-stu-id="dab7d-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dab7d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dab7d-133">JSON representation</span></span>

<span data-ttu-id="dab7d-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dab7d-134">The following is a JSON representation of the resource.</span></span>

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
