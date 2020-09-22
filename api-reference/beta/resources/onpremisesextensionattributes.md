---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的 **onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性的属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: 2729d6d624f1bde304425229ccf4ae7df8ddf781
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052586"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="e8fac-103">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="e8fac-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="e8fac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8fac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8fac-105">[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="e8fac-106">对于 **onPremisesSyncEnabled** 用户，此属性集的权威来源是同步到 Azure AD 的本地 Active Directory，并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="e8fac-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="e8fac-107">对于仅限云的用户 (其中 **onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-107">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="e8fac-108">**注意：** 这些扩展属性也称为 Exchange 自定义属性1-15。</span><span class="sxs-lookup"><span data-stu-id="e8fac-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="e8fac-109">属性</span><span class="sxs-lookup"><span data-stu-id="e8fac-109">Properties</span></span>
| <span data-ttu-id="e8fac-110">属性</span><span class="sxs-lookup"><span data-stu-id="e8fac-110">Property</span></span>     | <span data-ttu-id="e8fac-111">类型</span><span class="sxs-lookup"><span data-stu-id="e8fac-111">Type</span></span>   |<span data-ttu-id="e8fac-112">说明</span><span class="sxs-lookup"><span data-stu-id="e8fac-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8fac-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="e8fac-113">extensionAttribute1</span></span>|<span data-ttu-id="e8fac-114">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-114">String</span></span>| <span data-ttu-id="e8fac-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="e8fac-116">extensionAttribute2</span></span>|<span data-ttu-id="e8fac-117">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-117">String</span></span>| <span data-ttu-id="e8fac-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="e8fac-119">extensionAttribute3</span></span>|<span data-ttu-id="e8fac-120">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-120">String</span></span>| <span data-ttu-id="e8fac-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="e8fac-122">extensionAttribute4</span></span>|<span data-ttu-id="e8fac-123">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-123">String</span></span>| <span data-ttu-id="e8fac-124">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="e8fac-125">extensionAttribute5</span></span>|<span data-ttu-id="e8fac-126">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-126">String</span></span>| <span data-ttu-id="e8fac-127">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="e8fac-128">extensionAttribute6</span></span>|<span data-ttu-id="e8fac-129">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-129">String</span></span>| <span data-ttu-id="e8fac-130">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="e8fac-131">extensionAttribute7</span></span>|<span data-ttu-id="e8fac-132">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-132">String</span></span>| <span data-ttu-id="e8fac-133">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="e8fac-134">extensionAttribute8</span></span>|<span data-ttu-id="e8fac-135">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-135">String</span></span>| <span data-ttu-id="e8fac-136">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="e8fac-137">extensionAttribute9</span></span>|<span data-ttu-id="e8fac-138">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-138">String</span></span>| <span data-ttu-id="e8fac-139">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="e8fac-140">extensionAttribute10</span></span>|<span data-ttu-id="e8fac-141">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-141">String</span></span>| <span data-ttu-id="e8fac-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="e8fac-143">extensionAttribute11</span></span>|<span data-ttu-id="e8fac-144">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-144">String</span></span>| <span data-ttu-id="e8fac-145">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="e8fac-146">extensionAttribute12</span></span>|<span data-ttu-id="e8fac-147">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-147">String</span></span>| <span data-ttu-id="e8fac-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="e8fac-149">extensionAttribute13</span></span>|<span data-ttu-id="e8fac-150">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-150">String</span></span>| <span data-ttu-id="e8fac-151">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="e8fac-152">extensionAttribute14</span></span>|<span data-ttu-id="e8fac-153">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-153">String</span></span>| <span data-ttu-id="e8fac-154">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e8fac-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="e8fac-155">extensionAttribute15</span></span>|<span data-ttu-id="e8fac-156">String</span><span class="sxs-lookup"><span data-stu-id="e8fac-156">String</span></span>| <span data-ttu-id="e8fac-157">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="e8fac-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e8fac-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e8fac-158">JSON representation</span></span>

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


