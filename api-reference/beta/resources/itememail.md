---
title: itemEmail 资源类型
description: itemEmail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aaf58bd7e20caeb418946814daa7ca8f7bb9bfa3
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229414"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="74365-103">itemEmail 资源类型</span><span class="sxs-lookup"><span data-stu-id="74365-103">itemEmail resource type</span></span>

<span data-ttu-id="74365-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74365-105">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="74365-105">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="74365-106">方法</span><span class="sxs-lookup"><span data-stu-id="74365-106">Methods</span></span>

| <span data-ttu-id="74365-107">方法</span><span class="sxs-lookup"><span data-stu-id="74365-107">Method</span></span>                                   | <span data-ttu-id="74365-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="74365-108">Return Type</span></span>               | <span data-ttu-id="74365-109">说明</span><span class="sxs-lookup"><span data-stu-id="74365-109">Description</span></span>                                                      |
|:-----------------------------------------|:--------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="74365-110">获取</span><span class="sxs-lookup"><span data-stu-id="74365-110">Get</span></span>](../api/itememail-get.md)           | [<span data-ttu-id="74365-111">itemEmail</span><span class="sxs-lookup"><span data-stu-id="74365-111">itemEmail</span></span>](itememail.md) | <span data-ttu-id="74365-112">读取**itemEmail**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74365-112">Read properties and relationships of an **itemEmail** object.</span></span>    |
| [<span data-ttu-id="74365-113">更新</span><span class="sxs-lookup"><span data-stu-id="74365-113">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="74365-114">itemEmail</span><span class="sxs-lookup"><span data-stu-id="74365-114">itemEmail</span></span>](itememail.md) | <span data-ttu-id="74365-115">更新**itemEmail**对象。</span><span class="sxs-lookup"><span data-stu-id="74365-115">Update an **itemEmail** object.</span></span>                                  |
| [<span data-ttu-id="74365-116">删除</span><span class="sxs-lookup"><span data-stu-id="74365-116">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="74365-117">无</span><span class="sxs-lookup"><span data-stu-id="74365-117">None</span></span>                      | <span data-ttu-id="74365-118">删除**itemEmail**对象。</span><span class="sxs-lookup"><span data-stu-id="74365-118">Delete an **itemEmail** object.</span></span>                                  |

## <a name="properties"></a><span data-ttu-id="74365-119">属性</span><span class="sxs-lookup"><span data-stu-id="74365-119">Properties</span></span>

| <span data-ttu-id="74365-120">属性</span><span class="sxs-lookup"><span data-stu-id="74365-120">Property</span></span>     | <span data-ttu-id="74365-121">类型</span><span class="sxs-lookup"><span data-stu-id="74365-121">Type</span></span>        | <span data-ttu-id="74365-122">说明</span><span class="sxs-lookup"><span data-stu-id="74365-122">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="74365-123">address</span><span class="sxs-lookup"><span data-stu-id="74365-123">address</span></span>       |<span data-ttu-id="74365-124">String</span><span class="sxs-lookup"><span data-stu-id="74365-124">String</span></span>       | <span data-ttu-id="74365-125">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="74365-125">The email address itself.</span></span>                                                 |
|<span data-ttu-id="74365-126">displayName</span><span class="sxs-lookup"><span data-stu-id="74365-126">displayName</span></span>   |<span data-ttu-id="74365-127">String</span><span class="sxs-lookup"><span data-stu-id="74365-127">String</span></span>       | <span data-ttu-id="74365-128">用户与特定电子邮件地址相关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="74365-128">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="74365-129">类型</span><span class="sxs-lookup"><span data-stu-id="74365-129">type</span></span>          |<span data-ttu-id="74365-130">字符串</span><span class="sxs-lookup"><span data-stu-id="74365-130">string</span></span>       | <span data-ttu-id="74365-131">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="74365-131">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="74365-132">关系</span><span class="sxs-lookup"><span data-stu-id="74365-132">Relationships</span></span>

<span data-ttu-id="74365-133">无</span><span class="sxs-lookup"><span data-stu-id="74365-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74365-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74365-134">JSON representation</span></span>

<span data-ttu-id="74365-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74365-135">The following is a JSON representation of the resource.</span></span>

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
