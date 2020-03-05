---
title: itemPhone 资源类型
description: itemPhone 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48c585a05043b4f17e5e7406eb44b9150b5e5bdc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523063"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="907c1-103">itemPhone 资源类型</span><span class="sxs-lookup"><span data-stu-id="907c1-103">itemPhone resource type</span></span>

<span data-ttu-id="907c1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="907c1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="907c1-105">表示有关与各种服务中的用户关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="907c1-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="907c1-106">方法</span><span class="sxs-lookup"><span data-stu-id="907c1-106">Methods</span></span>

| <span data-ttu-id="907c1-107">方法</span><span class="sxs-lookup"><span data-stu-id="907c1-107">Method</span></span>                                     | <span data-ttu-id="907c1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="907c1-108">Return Type</span></span>               | <span data-ttu-id="907c1-109">说明</span><span class="sxs-lookup"><span data-stu-id="907c1-109">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="907c1-110">获取 itemPhone</span><span class="sxs-lookup"><span data-stu-id="907c1-110">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="907c1-111">itemPhone</span><span class="sxs-lookup"><span data-stu-id="907c1-111">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="907c1-112">读取**itemPhone**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="907c1-112">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="907c1-113">更新 itemPhone</span><span class="sxs-lookup"><span data-stu-id="907c1-113">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="907c1-114">itemPhone</span><span class="sxs-lookup"><span data-stu-id="907c1-114">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="907c1-115">更新**itemPhone**对象。</span><span class="sxs-lookup"><span data-stu-id="907c1-115">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="907c1-116">删除 itemPhone</span><span class="sxs-lookup"><span data-stu-id="907c1-116">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="907c1-117">无</span><span class="sxs-lookup"><span data-stu-id="907c1-117">None</span></span>                      | <span data-ttu-id="907c1-118">删除**itemPhone**对象。</span><span class="sxs-lookup"><span data-stu-id="907c1-118">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="907c1-119">属性</span><span class="sxs-lookup"><span data-stu-id="907c1-119">Properties</span></span>

| <span data-ttu-id="907c1-120">属性</span><span class="sxs-lookup"><span data-stu-id="907c1-120">Property</span></span>     | <span data-ttu-id="907c1-121">类型</span><span class="sxs-lookup"><span data-stu-id="907c1-121">Type</span></span>        | <span data-ttu-id="907c1-122">说明</span><span class="sxs-lookup"><span data-stu-id="907c1-122">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="907c1-123">displayName</span><span class="sxs-lookup"><span data-stu-id="907c1-123">displayName</span></span>   |<span data-ttu-id="907c1-124">String</span><span class="sxs-lookup"><span data-stu-id="907c1-124">String</span></span>       | <span data-ttu-id="907c1-125">包含电话号码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="907c1-125">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="907c1-126">number</span><span class="sxs-lookup"><span data-stu-id="907c1-126">number</span></span>        |<span data-ttu-id="907c1-127">String</span><span class="sxs-lookup"><span data-stu-id="907c1-127">String</span></span>       | <span data-ttu-id="907c1-128">包含电话号码。</span><span class="sxs-lookup"><span data-stu-id="907c1-128">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="907c1-129">类型</span><span class="sxs-lookup"><span data-stu-id="907c1-129">type</span></span>          |<span data-ttu-id="907c1-130">字符串</span><span class="sxs-lookup"><span data-stu-id="907c1-130">string</span></span>       | <span data-ttu-id="907c1-131">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="907c1-131">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="907c1-132">关系</span><span class="sxs-lookup"><span data-stu-id="907c1-132">Relationships</span></span>

<span data-ttu-id="907c1-133">无</span><span class="sxs-lookup"><span data-stu-id="907c1-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="907c1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="907c1-134">JSON representation</span></span>

<span data-ttu-id="907c1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="907c1-135">The following is a JSON representation of the resource.</span></span>

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
