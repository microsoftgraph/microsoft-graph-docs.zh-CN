---
title: onPremisesExtensionAttributes 资源类型
description: user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 对于 **onPremisesSyncEnabled** 用户，这组属性在本地 Active Directory 中托管并同步到 Azure AD，并且为只读。 对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以通过 Exchange Online 设置这些属性。 这些属性在 Microsoft Graph 中是只读的。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: f21369156e1a1337d16d64be40bd6de210bd56d2
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766103"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="fcadd-106">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcadd-106">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="fcadd-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcadd-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcadd-108">user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="fcadd-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="fcadd-109">对于 **onPremisesSyncEnabled** 用户，这组属性的颁发机构是同步到 Azure AD 且只读的本地 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="fcadd-109">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="fcadd-110">对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以通过 Exchange Online 设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties can be set over Exchange Online.</span></span> <span data-ttu-id="fcadd-111">这些属性在 Microsoft Graph 中是只读的。</span><span class="sxs-lookup"><span data-stu-id="fcadd-111">The attributes are read only in Microsoft Graph.</span></span>

> <span data-ttu-id="fcadd-112">**注意：** 这些扩展属性也称为 Exchange 自定义属性 1-15。</span><span class="sxs-lookup"><span data-stu-id="fcadd-112">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="fcadd-113">属性</span><span class="sxs-lookup"><span data-stu-id="fcadd-113">Properties</span></span>
| <span data-ttu-id="fcadd-114">属性</span><span class="sxs-lookup"><span data-stu-id="fcadd-114">Property</span></span>     | <span data-ttu-id="fcadd-115">类型</span><span class="sxs-lookup"><span data-stu-id="fcadd-115">Type</span></span>   |<span data-ttu-id="fcadd-116">说明</span><span class="sxs-lookup"><span data-stu-id="fcadd-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcadd-117">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="fcadd-117">extensionAttribute1</span></span>|<span data-ttu-id="fcadd-118">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-118">String</span></span>| <span data-ttu-id="fcadd-119">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-119">First customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-120">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="fcadd-120">extensionAttribute2</span></span>|<span data-ttu-id="fcadd-121">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-121">String</span></span>| <span data-ttu-id="fcadd-122">第二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-122">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-123">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="fcadd-123">extensionAttribute3</span></span>|<span data-ttu-id="fcadd-124">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-124">String</span></span>| <span data-ttu-id="fcadd-125">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-125">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-126">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="fcadd-126">extensionAttribute4</span></span>|<span data-ttu-id="fcadd-127">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-127">String</span></span>| <span data-ttu-id="fcadd-128">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-128">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-129">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="fcadd-129">extensionAttribute5</span></span>|<span data-ttu-id="fcadd-130">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-130">String</span></span>| <span data-ttu-id="fcadd-131">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-131">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-132">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="fcadd-132">extensionAttribute6</span></span>|<span data-ttu-id="fcadd-133">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-133">String</span></span>| <span data-ttu-id="fcadd-134">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-134">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-135">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="fcadd-135">extensionAttribute7</span></span>|<span data-ttu-id="fcadd-136">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-136">String</span></span>| <span data-ttu-id="fcadd-137">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-137">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-138">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="fcadd-138">extensionAttribute8</span></span>|<span data-ttu-id="fcadd-139">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-139">String</span></span>| <span data-ttu-id="fcadd-140">第八个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-140">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-141">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="fcadd-141">extensionAttribute9</span></span>|<span data-ttu-id="fcadd-142">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-142">String</span></span>| <span data-ttu-id="fcadd-143">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-143">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-144">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="fcadd-144">extensionAttribute10</span></span>|<span data-ttu-id="fcadd-145">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-145">String</span></span>| <span data-ttu-id="fcadd-146">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-146">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-147">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="fcadd-147">extensionAttribute11</span></span>|<span data-ttu-id="fcadd-148">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-148">String</span></span>| <span data-ttu-id="fcadd-149">第十一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-149">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-150">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="fcadd-150">extensionAttribute12</span></span>|<span data-ttu-id="fcadd-151">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-151">String</span></span>| <span data-ttu-id="fcadd-152">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-152">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-153">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="fcadd-153">extensionAttribute13</span></span>|<span data-ttu-id="fcadd-154">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-154">String</span></span>| <span data-ttu-id="fcadd-155">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-155">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-156">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="fcadd-156">extensionAttribute14</span></span>|<span data-ttu-id="fcadd-157">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-157">String</span></span>| <span data-ttu-id="fcadd-158">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-158">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="fcadd-159">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="fcadd-159">extensionAttribute15</span></span>|<span data-ttu-id="fcadd-160">String</span><span class="sxs-lookup"><span data-stu-id="fcadd-160">String</span></span>| <span data-ttu-id="fcadd-161">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fcadd-161">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fcadd-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcadd-162">JSON representation</span></span>

<span data-ttu-id="fcadd-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcadd-163">Here is a JSON representation of the resource</span></span>

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

