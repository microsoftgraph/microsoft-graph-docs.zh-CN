---
title: onPremisesExtensionAttributes 资源类型
description: 用户 **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 95d777140210070471c9578399e26e0eda3620d7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720583"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="aa9ae-103">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa9ae-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="aa9ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa9ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa9ae-105">用户 **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="aa9ae-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="aa9ae-106">对于 **onPremisesSyncEnabled** 用户，这组属性的颁发机构是同步到 Azure AD 且只读本地 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="aa9ae-107">对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-107">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="aa9ae-108">**注意：** 这些扩展属性也称为 Exchange 自定义属性 1-15。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="aa9ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="aa9ae-109">Properties</span></span>
| <span data-ttu-id="aa9ae-110">属性</span><span class="sxs-lookup"><span data-stu-id="aa9ae-110">Property</span></span>     | <span data-ttu-id="aa9ae-111">类型</span><span class="sxs-lookup"><span data-stu-id="aa9ae-111">Type</span></span>   |<span data-ttu-id="aa9ae-112">说明</span><span class="sxs-lookup"><span data-stu-id="aa9ae-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa9ae-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="aa9ae-113">extensionAttribute1</span></span>|<span data-ttu-id="aa9ae-114">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-114">String</span></span>| <span data-ttu-id="aa9ae-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="aa9ae-116">extensionAttribute2</span></span>|<span data-ttu-id="aa9ae-117">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-117">String</span></span>| <span data-ttu-id="aa9ae-118">第二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="aa9ae-119">extensionAttribute3</span></span>|<span data-ttu-id="aa9ae-120">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-120">String</span></span>| <span data-ttu-id="aa9ae-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="aa9ae-122">extensionAttribute4</span></span>|<span data-ttu-id="aa9ae-123">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-123">String</span></span>| <span data-ttu-id="aa9ae-124">第四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="aa9ae-125">extensionAttribute5</span></span>|<span data-ttu-id="aa9ae-126">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-126">String</span></span>| <span data-ttu-id="aa9ae-127">第五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="aa9ae-128">extensionAttribute6</span></span>|<span data-ttu-id="aa9ae-129">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-129">String</span></span>| <span data-ttu-id="aa9ae-130">第六个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="aa9ae-131">extensionAttribute7</span></span>|<span data-ttu-id="aa9ae-132">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-132">String</span></span>| <span data-ttu-id="aa9ae-133">第七个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="aa9ae-134">extensionAttribute8</span></span>|<span data-ttu-id="aa9ae-135">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-135">String</span></span>| <span data-ttu-id="aa9ae-136">第八个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="aa9ae-137">extensionAttribute9</span></span>|<span data-ttu-id="aa9ae-138">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-138">String</span></span>| <span data-ttu-id="aa9ae-139">第九个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="aa9ae-140">extensionAttribute10</span></span>|<span data-ttu-id="aa9ae-141">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-141">String</span></span>| <span data-ttu-id="aa9ae-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="aa9ae-143">extensionAttribute11</span></span>|<span data-ttu-id="aa9ae-144">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-144">String</span></span>| <span data-ttu-id="aa9ae-145">第十一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="aa9ae-146">extensionAttribute12</span></span>|<span data-ttu-id="aa9ae-147">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-147">String</span></span>| <span data-ttu-id="aa9ae-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="aa9ae-149">extensionAttribute13</span></span>|<span data-ttu-id="aa9ae-150">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-150">String</span></span>| <span data-ttu-id="aa9ae-151">第十三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="aa9ae-152">extensionAttribute14</span></span>|<span data-ttu-id="aa9ae-153">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-153">String</span></span>| <span data-ttu-id="aa9ae-154">第十四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="aa9ae-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="aa9ae-155">extensionAttribute15</span></span>|<span data-ttu-id="aa9ae-156">String</span><span class="sxs-lookup"><span data-stu-id="aa9ae-156">String</span></span>| <span data-ttu-id="aa9ae-157">第十五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="aa9ae-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aa9ae-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa9ae-158">JSON representation</span></span>

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


