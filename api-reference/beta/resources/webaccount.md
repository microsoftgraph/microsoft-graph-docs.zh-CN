---
title: webAccount 资源类型
description: webAccount 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ceb282dbcf0370e5eca2001b582660bdcaa1f1aa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519447"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="f6197-103">webAccount 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6197-103">webAccount resource type</span></span>

<span data-ttu-id="f6197-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f6197-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6197-105">表示用户已将其添加到其用户[配置文件](profile.md)中的 web 帐户。</span><span class="sxs-lookup"><span data-stu-id="f6197-105">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="f6197-106">此资源类型继承自[itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="f6197-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f6197-107">方法</span><span class="sxs-lookup"><span data-stu-id="f6197-107">Methods</span></span>

| <span data-ttu-id="f6197-108">方法</span><span class="sxs-lookup"><span data-stu-id="f6197-108">Method</span></span>                                     | <span data-ttu-id="f6197-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f6197-109">Return Type</span></span>                 | <span data-ttu-id="f6197-110">说明</span><span class="sxs-lookup"><span data-stu-id="f6197-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="f6197-111">获取 webAccount</span><span class="sxs-lookup"><span data-stu-id="f6197-111">Get webAccount</span></span>](../api/webaccount-get.md) | [<span data-ttu-id="f6197-112">webAccount</span><span class="sxs-lookup"><span data-stu-id="f6197-112">webAccount</span></span>](webaccount.md) | <span data-ttu-id="f6197-113">读取**webAccount**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f6197-113">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="f6197-114">更新 webAccount</span><span class="sxs-lookup"><span data-stu-id="f6197-114">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="f6197-115">webAccount</span><span class="sxs-lookup"><span data-stu-id="f6197-115">webAccount</span></span>](webaccount.md) | <span data-ttu-id="f6197-116">更新**webAccount**对象。</span><span class="sxs-lookup"><span data-stu-id="f6197-116">Update a **webAccount** object.</span></span>                               |
| [<span data-ttu-id="f6197-117">删除 webAccount</span><span class="sxs-lookup"><span data-stu-id="f6197-117">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="f6197-118">无</span><span class="sxs-lookup"><span data-stu-id="f6197-118">None</span></span>                        | <span data-ttu-id="f6197-119">删除**webAccount**对象。</span><span class="sxs-lookup"><span data-stu-id="f6197-119">Delete a **webAccount** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="f6197-120">属性</span><span class="sxs-lookup"><span data-stu-id="f6197-120">Properties</span></span>

| <span data-ttu-id="f6197-121">属性</span><span class="sxs-lookup"><span data-stu-id="f6197-121">Property</span></span>     | <span data-ttu-id="f6197-122">类型</span><span class="sxs-lookup"><span data-stu-id="f6197-122">Type</span></span>                                      | <span data-ttu-id="f6197-123">说明</span><span class="sxs-lookup"><span data-stu-id="f6197-123">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="f6197-124">说明</span><span class="sxs-lookup"><span data-stu-id="f6197-124">description</span></span>   |<span data-ttu-id="f6197-125">字符串</span><span class="sxs-lookup"><span data-stu-id="f6197-125">String</span></span>                                     | <span data-ttu-id="f6197-126">包含用户为所引用服务上的帐户提供的说明。</span><span class="sxs-lookup"><span data-stu-id="f6197-126">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="f6197-127">service</span><span class="sxs-lookup"><span data-stu-id="f6197-127">service</span></span>       |[<span data-ttu-id="f6197-128">serviceInformation</span><span class="sxs-lookup"><span data-stu-id="f6197-128">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="f6197-129">包含有关要关联的服务的基本详细信息。</span><span class="sxs-lookup"><span data-stu-id="f6197-129">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="f6197-130">statusMessage</span><span class="sxs-lookup"><span data-stu-id="f6197-130">statusMessage</span></span> |<span data-ttu-id="f6197-131">String</span><span class="sxs-lookup"><span data-stu-id="f6197-131">String</span></span>                                     | <span data-ttu-id="f6197-132">包含来自云服务的状态邮件（如果提供或已同步）。</span><span class="sxs-lookup"><span data-stu-id="f6197-132">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="f6197-133">userId</span><span class="sxs-lookup"><span data-stu-id="f6197-133">userId</span></span>        |<span data-ttu-id="f6197-134">String</span><span class="sxs-lookup"><span data-stu-id="f6197-134">String</span></span>                                     | <span data-ttu-id="f6197-135">为 webaccount 显示的用户名。</span><span class="sxs-lookup"><span data-stu-id="f6197-135">The user name  displayed for the webaccount.</span></span>                                    |
|<span data-ttu-id="f6197-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="f6197-136">webUrl</span></span>        |<span data-ttu-id="f6197-137">String</span><span class="sxs-lookup"><span data-stu-id="f6197-137">String</span></span>                                     | <span data-ttu-id="f6197-138">包含指向云服务上的用户配置文件的链接（如果存在）。</span><span class="sxs-lookup"><span data-stu-id="f6197-138">Contains a link to the user's profile on the cloud service if one exists.</span></span>                       |

## <a name="relationships"></a><span data-ttu-id="f6197-139">关系</span><span class="sxs-lookup"><span data-stu-id="f6197-139">Relationships</span></span>

<span data-ttu-id="f6197-140">无</span><span class="sxs-lookup"><span data-stu-id="f6197-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6197-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6197-141">JSON representation</span></span>

<span data-ttu-id="f6197-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6197-142">The following is a JSON representation of the resource.</span></span>

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
