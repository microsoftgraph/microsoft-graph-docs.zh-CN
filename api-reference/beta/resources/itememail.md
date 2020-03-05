---
title: itemEmail 资源类型
description: itemEmail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a18d72fb44f373b6cee1047cc2eed5f0c18a1d0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523077"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="8dff5-103">itemEmail 资源类型</span><span class="sxs-lookup"><span data-stu-id="8dff5-103">itemEmail resource type</span></span>

<span data-ttu-id="8dff5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8dff5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dff5-105">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8dff5-105">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="8dff5-106">方法</span><span class="sxs-lookup"><span data-stu-id="8dff5-106">Methods</span></span>

| <span data-ttu-id="8dff5-107">方法</span><span class="sxs-lookup"><span data-stu-id="8dff5-107">Method</span></span>                                   | <span data-ttu-id="8dff5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8dff5-108">Return Type</span></span>               | <span data-ttu-id="8dff5-109">说明</span><span class="sxs-lookup"><span data-stu-id="8dff5-109">Description</span></span>                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="8dff5-110">获取</span><span class="sxs-lookup"><span data-stu-id="8dff5-110">Get</span></span>](../api/itememail-get.md) | [<span data-ttu-id="8dff5-111">itemEmail</span><span class="sxs-lookup"><span data-stu-id="8dff5-111">itemEmail</span></span>](itememail.md) | <span data-ttu-id="8dff5-112">读取**itemEmail**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8dff5-112">Read properties and relationships of an **itemEmail** object.</span></span> |
| [<span data-ttu-id="8dff5-113">更新</span><span class="sxs-lookup"><span data-stu-id="8dff5-113">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="8dff5-114">itemEmail</span><span class="sxs-lookup"><span data-stu-id="8dff5-114">itemEmail</span></span>](itememail.md) | <span data-ttu-id="8dff5-115">更新**itemEmail**对象。</span><span class="sxs-lookup"><span data-stu-id="8dff5-115">Update an **itemEmail** object.</span></span>                               |
| [<span data-ttu-id="8dff5-116">删除</span><span class="sxs-lookup"><span data-stu-id="8dff5-116">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="8dff5-117">无</span><span class="sxs-lookup"><span data-stu-id="8dff5-117">None</span></span>                      | <span data-ttu-id="8dff5-118">删除**itemEmail**对象。</span><span class="sxs-lookup"><span data-stu-id="8dff5-118">Delete an **itemEmail** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="8dff5-119">属性</span><span class="sxs-lookup"><span data-stu-id="8dff5-119">Properties</span></span>

| <span data-ttu-id="8dff5-120">属性</span><span class="sxs-lookup"><span data-stu-id="8dff5-120">Property</span></span>     | <span data-ttu-id="8dff5-121">类型</span><span class="sxs-lookup"><span data-stu-id="8dff5-121">Type</span></span>        | <span data-ttu-id="8dff5-122">说明</span><span class="sxs-lookup"><span data-stu-id="8dff5-122">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="8dff5-123">address</span><span class="sxs-lookup"><span data-stu-id="8dff5-123">address</span></span>       |<span data-ttu-id="8dff5-124">String</span><span class="sxs-lookup"><span data-stu-id="8dff5-124">String</span></span>       | <span data-ttu-id="8dff5-125">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="8dff5-125">The email address itself.</span></span>                                                 |
|<span data-ttu-id="8dff5-126">displayName</span><span class="sxs-lookup"><span data-stu-id="8dff5-126">displayName</span></span>   |<span data-ttu-id="8dff5-127">String</span><span class="sxs-lookup"><span data-stu-id="8dff5-127">String</span></span>       | <span data-ttu-id="8dff5-128">用户与特定电子邮件地址相关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="8dff5-128">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="8dff5-129">类型</span><span class="sxs-lookup"><span data-stu-id="8dff5-129">type</span></span>          |<span data-ttu-id="8dff5-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8dff5-130">string</span></span>       | <span data-ttu-id="8dff5-131">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="8dff5-131">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="8dff5-132">关系</span><span class="sxs-lookup"><span data-stu-id="8dff5-132">Relationships</span></span>

<span data-ttu-id="8dff5-133">无</span><span class="sxs-lookup"><span data-stu-id="8dff5-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8dff5-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8dff5-134">JSON representation</span></span>

<span data-ttu-id="8dff5-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8dff5-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemEmail",
  "baseType": ""
}-->

```json
{
  "address": "String",
  "displayName": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemEmail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
