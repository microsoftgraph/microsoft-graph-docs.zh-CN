---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 1035674a6ce5d9f2c0a1a8b2cd35896c92ec7147
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863752"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="b804d-103">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="b804d-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="b804d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b804d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b804d-105">[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="b804d-106">对于**onPremisesSyncEnabled**用户，此属性集的权威来源是同步到 Azure AD 的本地 Active Directory，并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="b804d-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="b804d-107">对于仅限云的用户（其中**onPremisesSyncEnabled**为 false），可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-107">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="b804d-108">**注意：** 这些扩展属性也称为 Exchange 自定义属性1-15。</span><span class="sxs-lookup"><span data-stu-id="b804d-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="b804d-109">属性</span><span class="sxs-lookup"><span data-stu-id="b804d-109">Properties</span></span>
| <span data-ttu-id="b804d-110">属性</span><span class="sxs-lookup"><span data-stu-id="b804d-110">Property</span></span>     | <span data-ttu-id="b804d-111">类型</span><span class="sxs-lookup"><span data-stu-id="b804d-111">Type</span></span>   |<span data-ttu-id="b804d-112">Description</span><span class="sxs-lookup"><span data-stu-id="b804d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b804d-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="b804d-113">extensionAttribute1</span></span>|<span data-ttu-id="b804d-114">String</span><span class="sxs-lookup"><span data-stu-id="b804d-114">String</span></span>| <span data-ttu-id="b804d-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="b804d-116">extensionAttribute2</span></span>|<span data-ttu-id="b804d-117">String</span><span class="sxs-lookup"><span data-stu-id="b804d-117">String</span></span>| <span data-ttu-id="b804d-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="b804d-119">extensionAttribute3</span></span>|<span data-ttu-id="b804d-120">String</span><span class="sxs-lookup"><span data-stu-id="b804d-120">String</span></span>| <span data-ttu-id="b804d-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="b804d-122">extensionAttribute4</span></span>|<span data-ttu-id="b804d-123">String</span><span class="sxs-lookup"><span data-stu-id="b804d-123">String</span></span>| <span data-ttu-id="b804d-124">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="b804d-125">extensionAttribute5</span></span>|<span data-ttu-id="b804d-126">String</span><span class="sxs-lookup"><span data-stu-id="b804d-126">String</span></span>| <span data-ttu-id="b804d-127">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="b804d-128">extensionAttribute6</span></span>|<span data-ttu-id="b804d-129">String</span><span class="sxs-lookup"><span data-stu-id="b804d-129">String</span></span>| <span data-ttu-id="b804d-130">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="b804d-131">extensionAttribute7</span></span>|<span data-ttu-id="b804d-132">String</span><span class="sxs-lookup"><span data-stu-id="b804d-132">String</span></span>| <span data-ttu-id="b804d-133">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="b804d-134">extensionAttribute8</span></span>|<span data-ttu-id="b804d-135">String</span><span class="sxs-lookup"><span data-stu-id="b804d-135">String</span></span>| <span data-ttu-id="b804d-136">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="b804d-137">extensionAttribute9</span></span>|<span data-ttu-id="b804d-138">String</span><span class="sxs-lookup"><span data-stu-id="b804d-138">String</span></span>| <span data-ttu-id="b804d-139">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="b804d-140">extensionAttribute10</span></span>|<span data-ttu-id="b804d-141">String</span><span class="sxs-lookup"><span data-stu-id="b804d-141">String</span></span>| <span data-ttu-id="b804d-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="b804d-143">extensionAttribute11</span></span>|<span data-ttu-id="b804d-144">String</span><span class="sxs-lookup"><span data-stu-id="b804d-144">String</span></span>| <span data-ttu-id="b804d-145">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="b804d-146">extensionAttribute12</span></span>|<span data-ttu-id="b804d-147">String</span><span class="sxs-lookup"><span data-stu-id="b804d-147">String</span></span>| <span data-ttu-id="b804d-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="b804d-149">extensionAttribute13</span></span>|<span data-ttu-id="b804d-150">String</span><span class="sxs-lookup"><span data-stu-id="b804d-150">String</span></span>| <span data-ttu-id="b804d-151">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="b804d-152">extensionAttribute14</span></span>|<span data-ttu-id="b804d-153">String</span><span class="sxs-lookup"><span data-stu-id="b804d-153">String</span></span>| <span data-ttu-id="b804d-154">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="b804d-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="b804d-155">extensionAttribute15</span></span>|<span data-ttu-id="b804d-156">String</span><span class="sxs-lookup"><span data-stu-id="b804d-156">String</span></span>| <span data-ttu-id="b804d-157">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="b804d-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b804d-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b804d-158">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
