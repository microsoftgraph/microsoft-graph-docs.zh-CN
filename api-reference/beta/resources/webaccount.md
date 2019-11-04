---
title: webAccount 资源类型
description: webAccount 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 414e3f491736f51ee670390519241110bc81f66e
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950353"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="0b53b-103">webAccount 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b53b-103">webAccount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b53b-104">表示用户已将其添加到其用户[配置文件](profile.md)中的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="0b53b-104">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="0b53b-105">此资源类型继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="0b53b-105">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0b53b-106">方法</span><span class="sxs-lookup"><span data-stu-id="0b53b-106">Methods</span></span>

| <span data-ttu-id="0b53b-107">方法</span><span class="sxs-lookup"><span data-stu-id="0b53b-107">Method</span></span>                                     | <span data-ttu-id="0b53b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0b53b-108">Return Type</span></span>                 | <span data-ttu-id="0b53b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b53b-109">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="0b53b-110">获取 webAccount</span><span class="sxs-lookup"><span data-stu-id="0b53b-110">Get webAccount</span></span>](../api/webaccount-get.md) | [<span data-ttu-id="0b53b-111">webAccount</span><span class="sxs-lookup"><span data-stu-id="0b53b-111">webAccount</span></span>](webaccount.md) | <span data-ttu-id="0b53b-112">读取**webAccount**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0b53b-112">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="0b53b-113">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="0b53b-113">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="0b53b-114">webAccount</span><span class="sxs-lookup"><span data-stu-id="0b53b-114">webAccount</span></span>](webaccount.md) | <span data-ttu-id="0b53b-115">更新**webAccount**对象。</span><span class="sxs-lookup"><span data-stu-id="0b53b-115">Update a **webAccount** object.</span></span>                               |
| [<span data-ttu-id="0b53b-116">删除 webAccount</span><span class="sxs-lookup"><span data-stu-id="0b53b-116">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="0b53b-117">无</span><span class="sxs-lookup"><span data-stu-id="0b53b-117">None</span></span>                        | <span data-ttu-id="0b53b-118">删除**webAccount**对象。</span><span class="sxs-lookup"><span data-stu-id="0b53b-118">Delete a **webAccount** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="0b53b-119">属性</span><span class="sxs-lookup"><span data-stu-id="0b53b-119">Properties</span></span>

| <span data-ttu-id="0b53b-120">属性</span><span class="sxs-lookup"><span data-stu-id="0b53b-120">Property</span></span>     | <span data-ttu-id="0b53b-121">类型</span><span class="sxs-lookup"><span data-stu-id="0b53b-121">Type</span></span>                                      | <span data-ttu-id="0b53b-122">说明</span><span class="sxs-lookup"><span data-stu-id="0b53b-122">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="0b53b-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b53b-123">description</span></span>   |<span data-ttu-id="0b53b-124">字符串</span><span class="sxs-lookup"><span data-stu-id="0b53b-124">String</span></span>                                     | <span data-ttu-id="0b53b-125">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="0b53b-125">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="0b53b-126">service</span><span class="sxs-lookup"><span data-stu-id="0b53b-126">service</span></span>       |[<span data-ttu-id="0b53b-127">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="0b53b-127">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="0b53b-128">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="0b53b-128">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="0b53b-129">statusMessage</span><span class="sxs-lookup"><span data-stu-id="0b53b-129">statusMessage</span></span> |<span data-ttu-id="0b53b-130">String</span><span class="sxs-lookup"><span data-stu-id="0b53b-130">String</span></span>                                     | <span data-ttu-id="0b53b-131">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="0b53b-131">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="0b53b-132">userId</span><span class="sxs-lookup"><span data-stu-id="0b53b-132">userId</span></span>        |<span data-ttu-id="0b53b-133">String</span><span class="sxs-lookup"><span data-stu-id="0b53b-133">String</span></span>                                     | <span data-ttu-id="0b53b-134">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="0b53b-134">The user name  displayed for the webaccount.</span></span>                                    |
|<span data-ttu-id="0b53b-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="0b53b-135">webUrl</span></span>        |<span data-ttu-id="0b53b-136">String</span><span class="sxs-lookup"><span data-stu-id="0b53b-136">String</span></span>                                     | <span data-ttu-id="0b53b-137">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="0b53b-137">Contains a link to the user's profile on the cloud service if one exists.</span></span>                       |

## <a name="relationships"></a><span data-ttu-id="0b53b-138">关系</span><span class="sxs-lookup"><span data-stu-id="0b53b-138">Relationships</span></span>

<span data-ttu-id="0b53b-139">无</span><span class="sxs-lookup"><span data-stu-id="0b53b-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b53b-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b53b-140">JSON representation</span></span>

<span data-ttu-id="0b53b-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b53b-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
