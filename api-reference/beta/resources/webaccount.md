---
title: webAccount 资源类型
description: webAccount 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dbdae8f0035e92b1c5b74c0ef3f842d2eb5af37a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228864"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="1ff53-103">webAccount 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ff53-103">webAccount resource type</span></span>

<span data-ttu-id="1ff53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ff53-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ff53-105">表示用户已将其添加到其用户[配置文件](profile.md)中的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="1ff53-105">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="1ff53-106">此资源类型继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="1ff53-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1ff53-107">方法</span><span class="sxs-lookup"><span data-stu-id="1ff53-107">Methods</span></span>

| <span data-ttu-id="1ff53-108">方法</span><span class="sxs-lookup"><span data-stu-id="1ff53-108">Method</span></span>                                                | <span data-ttu-id="1ff53-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ff53-109">Return Type</span></span>                 | <span data-ttu-id="1ff53-110">说明</span><span class="sxs-lookup"><span data-stu-id="1ff53-110">Description</span></span>                                                       |
|:------------------------------------------------------|:----------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="1ff53-111">获取 webAccount</span><span class="sxs-lookup"><span data-stu-id="1ff53-111">Get webAccount</span></span>](../api/webaccount-get.md)            | [<span data-ttu-id="1ff53-112">webAccount</span><span class="sxs-lookup"><span data-stu-id="1ff53-112">webAccount</span></span>](webaccount.md) | <span data-ttu-id="1ff53-113">读取**webAccount**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ff53-113">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="1ff53-114">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="1ff53-114">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="1ff53-115">webAccount</span><span class="sxs-lookup"><span data-stu-id="1ff53-115">webAccount</span></span>](webaccount.md) | <span data-ttu-id="1ff53-116">更新**webAccount**对象。</span><span class="sxs-lookup"><span data-stu-id="1ff53-116">Update a **webAccount** object.</span></span>                                   |
| [<span data-ttu-id="1ff53-117">删除 webAccount</span><span class="sxs-lookup"><span data-stu-id="1ff53-117">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="1ff53-118">无</span><span class="sxs-lookup"><span data-stu-id="1ff53-118">None</span></span>                        | <span data-ttu-id="1ff53-119">删除**webAccount**对象。</span><span class="sxs-lookup"><span data-stu-id="1ff53-119">Delete a **webAccount** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="1ff53-120">属性</span><span class="sxs-lookup"><span data-stu-id="1ff53-120">Properties</span></span>

| <span data-ttu-id="1ff53-121">属性</span><span class="sxs-lookup"><span data-stu-id="1ff53-121">Property</span></span>     | <span data-ttu-id="1ff53-122">类型</span><span class="sxs-lookup"><span data-stu-id="1ff53-122">Type</span></span>                                      | <span data-ttu-id="1ff53-123">说明</span><span class="sxs-lookup"><span data-stu-id="1ff53-123">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="1ff53-124">说明</span><span class="sxs-lookup"><span data-stu-id="1ff53-124">description</span></span>   |<span data-ttu-id="1ff53-125">字符串</span><span class="sxs-lookup"><span data-stu-id="1ff53-125">String</span></span>                                     | <span data-ttu-id="1ff53-126">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="1ff53-126">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="1ff53-127">service</span><span class="sxs-lookup"><span data-stu-id="1ff53-127">service</span></span>       |[<span data-ttu-id="1ff53-128">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="1ff53-128">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="1ff53-129">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="1ff53-129">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="1ff53-130">statusMessage</span><span class="sxs-lookup"><span data-stu-id="1ff53-130">statusMessage</span></span> |<span data-ttu-id="1ff53-131">String</span><span class="sxs-lookup"><span data-stu-id="1ff53-131">String</span></span>                                     | <span data-ttu-id="1ff53-132">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="1ff53-132">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="1ff53-133">userId</span><span class="sxs-lookup"><span data-stu-id="1ff53-133">userId</span></span>        |<span data-ttu-id="1ff53-134">String</span><span class="sxs-lookup"><span data-stu-id="1ff53-134">String</span></span>                                     | <span data-ttu-id="1ff53-135">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="1ff53-135">The user name  displayed for the webaccount.</span></span>                                                   |
|<span data-ttu-id="1ff53-136">WebUrl</span><span class="sxs-lookup"><span data-stu-id="1ff53-136">webUrl</span></span>        |<span data-ttu-id="1ff53-137">String</span><span class="sxs-lookup"><span data-stu-id="1ff53-137">String</span></span>                                     | <span data-ttu-id="1ff53-138">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="1ff53-138">Contains a link to the user's profile on the cloud service if one exists.</span></span>                      |

## <a name="relationships"></a><span data-ttu-id="1ff53-139">关系</span><span class="sxs-lookup"><span data-stu-id="1ff53-139">Relationships</span></span>

<span data-ttu-id="1ff53-140">无</span><span class="sxs-lookup"><span data-stu-id="1ff53-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ff53-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ff53-141">JSON representation</span></span>

<span data-ttu-id="1ff53-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ff53-142">The following is a JSON representation of the resource.</span></span>

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
