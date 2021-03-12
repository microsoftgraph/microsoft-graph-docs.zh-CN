---
title: onPremisesExtensionAttributes 资源类型
description: user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 对于 **onPremisesSyncEnabled** 用户，这组属性在本地 Active Directory 中托管并同步到 Azure AD，并且为只读。 对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: c8e44879b3248cab502ee2aeabdaa732a2b35e1f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718955"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="548a7-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="548a7-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="548a7-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="548a7-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="548a7-107">user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="548a7-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="548a7-108">对于 **onPremisesSyncEnabled** 用户，这组属性的颁发机构是同步到 Azure AD 且只读的本地 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="548a7-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="548a7-109">对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="548a7-110">**注意：** 这些扩展属性也称为 Exchange 自定义属性 1-15。</span><span class="sxs-lookup"><span data-stu-id="548a7-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="548a7-111">属性</span><span class="sxs-lookup"><span data-stu-id="548a7-111">Properties</span></span>
| <span data-ttu-id="548a7-112">属性</span><span class="sxs-lookup"><span data-stu-id="548a7-112">Property</span></span>     | <span data-ttu-id="548a7-113">类型</span><span class="sxs-lookup"><span data-stu-id="548a7-113">Type</span></span>   |<span data-ttu-id="548a7-114">说明</span><span class="sxs-lookup"><span data-stu-id="548a7-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="548a7-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="548a7-115">extensionAttribute1</span></span>|<span data-ttu-id="548a7-116">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-116">String</span></span>| <span data-ttu-id="548a7-117">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="548a7-118">extensionAttribute2</span></span>|<span data-ttu-id="548a7-119">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-119">String</span></span>| <span data-ttu-id="548a7-120">第二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="548a7-121">extensionAttribute3</span></span>|<span data-ttu-id="548a7-122">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-122">String</span></span>| <span data-ttu-id="548a7-123">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="548a7-124">extensionAttribute4</span></span>|<span data-ttu-id="548a7-125">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-125">String</span></span>| <span data-ttu-id="548a7-126">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="548a7-127">extensionAttribute5</span></span>|<span data-ttu-id="548a7-128">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-128">String</span></span>| <span data-ttu-id="548a7-129">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="548a7-130">extensionAttribute6</span></span>|<span data-ttu-id="548a7-131">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-131">String</span></span>| <span data-ttu-id="548a7-132">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="548a7-133">extensionAttribute7</span></span>|<span data-ttu-id="548a7-134">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-134">String</span></span>| <span data-ttu-id="548a7-135">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="548a7-136">extensionAttribute8</span></span>|<span data-ttu-id="548a7-137">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-137">String</span></span>| <span data-ttu-id="548a7-138">第八个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="548a7-139">extensionAttribute9</span></span>|<span data-ttu-id="548a7-140">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-140">String</span></span>| <span data-ttu-id="548a7-141">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="548a7-142">extensionAttribute10</span></span>|<span data-ttu-id="548a7-143">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-143">String</span></span>| <span data-ttu-id="548a7-144">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="548a7-145">extensionAttribute11</span></span>|<span data-ttu-id="548a7-146">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-146">String</span></span>| <span data-ttu-id="548a7-147">第十一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="548a7-148">extensionAttribute12</span></span>|<span data-ttu-id="548a7-149">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-149">String</span></span>| <span data-ttu-id="548a7-150">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="548a7-151">extensionAttribute13</span></span>|<span data-ttu-id="548a7-152">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-152">String</span></span>| <span data-ttu-id="548a7-153">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="548a7-154">extensionAttribute14</span></span>|<span data-ttu-id="548a7-155">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-155">String</span></span>| <span data-ttu-id="548a7-156">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="548a7-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="548a7-157">extensionAttribute15</span></span>|<span data-ttu-id="548a7-158">字符串</span><span class="sxs-lookup"><span data-stu-id="548a7-158">String</span></span>| <span data-ttu-id="548a7-159">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="548a7-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="548a7-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="548a7-160">JSON representation</span></span>

<span data-ttu-id="548a7-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="548a7-161">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

