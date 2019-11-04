---
title: itemEmail 资源类型
description: itemEmail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: eed73f61b281463848c8520ebdcdbc75ac26d29d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939332"
---
# <a name="itememail-resource-type"></a><span data-ttu-id="c3875-103">itemEmail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3875-103">itemEmail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3875-104">表示有关与用户相关联的电子邮件地址的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c3875-104">Represents detailed information about email addresses associated with the user.</span></span>

## <a name="methods"></a><span data-ttu-id="c3875-105">方法</span><span class="sxs-lookup"><span data-stu-id="c3875-105">Methods</span></span>

| <span data-ttu-id="c3875-106">方法</span><span class="sxs-lookup"><span data-stu-id="c3875-106">Method</span></span>                                   | <span data-ttu-id="c3875-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3875-107">Return Type</span></span>               | <span data-ttu-id="c3875-108">说明</span><span class="sxs-lookup"><span data-stu-id="c3875-108">Description</span></span>                                            |
|:-----------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="c3875-109">Get</span><span class="sxs-lookup"><span data-stu-id="c3875-109">Get</span></span>](../api/itememail-get.md) | [<span data-ttu-id="c3875-110">itemEmail</span><span class="sxs-lookup"><span data-stu-id="c3875-110">itemEmail</span></span>](itememail.md) | <span data-ttu-id="c3875-111">读取**itemEmail**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3875-111">Read properties and relationships of an **itemEmail** object.</span></span> |
| [<span data-ttu-id="c3875-112">Update</span><span class="sxs-lookup"><span data-stu-id="c3875-112">Update</span></span>](../api/itememail-update.md)     | [<span data-ttu-id="c3875-113">itemEmail</span><span class="sxs-lookup"><span data-stu-id="c3875-113">itemEmail</span></span>](itememail.md) | <span data-ttu-id="c3875-114">更新**itemEmail**对象。</span><span class="sxs-lookup"><span data-stu-id="c3875-114">Update an **itemEmail** object.</span></span>                               |
| [<span data-ttu-id="c3875-115">删除</span><span class="sxs-lookup"><span data-stu-id="c3875-115">Delete</span></span>](../api/itememail-delete.md)     | <span data-ttu-id="c3875-116">无</span><span class="sxs-lookup"><span data-stu-id="c3875-116">None</span></span>                      | <span data-ttu-id="c3875-117">删除**itemEmail**对象。</span><span class="sxs-lookup"><span data-stu-id="c3875-117">Delete an **itemEmail** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="c3875-118">属性</span><span class="sxs-lookup"><span data-stu-id="c3875-118">Properties</span></span>

| <span data-ttu-id="c3875-119">属性</span><span class="sxs-lookup"><span data-stu-id="c3875-119">Property</span></span>     | <span data-ttu-id="c3875-120">类型</span><span class="sxs-lookup"><span data-stu-id="c3875-120">Type</span></span>        | <span data-ttu-id="c3875-121">描述</span><span class="sxs-lookup"><span data-stu-id="c3875-121">Description</span></span>                                                               |
|:-------------|:------------|:--------------------------------------------------------------------------|
|<span data-ttu-id="c3875-122">address</span><span class="sxs-lookup"><span data-stu-id="c3875-122">address</span></span>       |<span data-ttu-id="c3875-123">String</span><span class="sxs-lookup"><span data-stu-id="c3875-123">String</span></span>       | <span data-ttu-id="c3875-124">电子邮件地址本身。</span><span class="sxs-lookup"><span data-stu-id="c3875-124">The email address itself.</span></span>                                                 |
|<span data-ttu-id="c3875-125">displayName</span><span class="sxs-lookup"><span data-stu-id="c3875-125">displayName</span></span>   |<span data-ttu-id="c3875-126">字符串</span><span class="sxs-lookup"><span data-stu-id="c3875-126">String</span></span>       | <span data-ttu-id="c3875-127">用户与特定电子邮件地址相关联的名称或标签。</span><span class="sxs-lookup"><span data-stu-id="c3875-127">The name or label a user has associated with a particular email address.</span></span>  |
|<span data-ttu-id="c3875-128">类型</span><span class="sxs-lookup"><span data-stu-id="c3875-128">type</span></span>          |<span data-ttu-id="c3875-129">字符串</span><span class="sxs-lookup"><span data-stu-id="c3875-129">string</span></span>       | <span data-ttu-id="c3875-130">可取值为：`unknown`、`work`、`personal`、`main`、`other`。</span><span class="sxs-lookup"><span data-stu-id="c3875-130">Possible values are: `unknown`, `work`, `personal`, `main`, `other`.</span></span>      |

## <a name="relationships"></a><span data-ttu-id="c3875-131">关系</span><span class="sxs-lookup"><span data-stu-id="c3875-131">Relationships</span></span>

<span data-ttu-id="c3875-132">无</span><span class="sxs-lookup"><span data-stu-id="c3875-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3875-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3875-133">JSON representation</span></span>

<span data-ttu-id="c3875-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3875-134">The following is a JSON representation of the resource.</span></span>

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
