---
title: onPremisesExtensionAttributes 资源类型
description: user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 对于 **onPremisesSyncEnabled** 用户，这组属性在本地 Active Directory 中托管并同步到 Azure AD，并且为只读。 对于仅云用户 (**onPremisesSyncEnabled** 为 false) ，可以通过以下方法设置Exchange Online。 这些属性在 Microsoft Graph。
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 3081b377a30bbf09131650517dcee61597dea597
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912045"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="221d5-106">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="221d5-106">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="221d5-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="221d5-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="221d5-108">user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="221d5-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="221d5-109">对于 **onPremisesSyncEnabled** 用户，这组属性的颁发机构是同步到 Azure AD 且只读的本地 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="221d5-109">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="221d5-110">对于仅云用户 (**onPremisesSyncEnabled**) ，可以在创建或更新期间设置 `false` [这些属性](../api/user-update.md)。 [](../api/user-post-users.md)</span><span class="sxs-lookup"><span data-stu-id="221d5-110">For a cloud-only user (where **onPremisesSyncEnabled** is `false`), these properties may be set during [creation](../api/user-post-users.md) or [update](../api/user-update.md).</span></span>

> <span data-ttu-id="221d5-111">**注意：** 这些扩展属性也称为自定义Exchange 1-15。</span><span class="sxs-lookup"><span data-stu-id="221d5-111">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="221d5-112">属性</span><span class="sxs-lookup"><span data-stu-id="221d5-112">Properties</span></span>
| <span data-ttu-id="221d5-113">属性</span><span class="sxs-lookup"><span data-stu-id="221d5-113">Property</span></span>     | <span data-ttu-id="221d5-114">类型</span><span class="sxs-lookup"><span data-stu-id="221d5-114">Type</span></span>   |<span data-ttu-id="221d5-115">说明</span><span class="sxs-lookup"><span data-stu-id="221d5-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="221d5-116">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="221d5-116">extensionAttribute1</span></span>|<span data-ttu-id="221d5-117">String</span><span class="sxs-lookup"><span data-stu-id="221d5-117">String</span></span>| <span data-ttu-id="221d5-118">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-118">First customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-119">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="221d5-119">extensionAttribute2</span></span>|<span data-ttu-id="221d5-120">String</span><span class="sxs-lookup"><span data-stu-id="221d5-120">String</span></span>| <span data-ttu-id="221d5-121">第二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-121">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-122">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="221d5-122">extensionAttribute3</span></span>|<span data-ttu-id="221d5-123">String</span><span class="sxs-lookup"><span data-stu-id="221d5-123">String</span></span>| <span data-ttu-id="221d5-124">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-124">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-125">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="221d5-125">extensionAttribute4</span></span>|<span data-ttu-id="221d5-126">String</span><span class="sxs-lookup"><span data-stu-id="221d5-126">String</span></span>| <span data-ttu-id="221d5-127">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-127">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-128">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="221d5-128">extensionAttribute5</span></span>|<span data-ttu-id="221d5-129">String</span><span class="sxs-lookup"><span data-stu-id="221d5-129">String</span></span>| <span data-ttu-id="221d5-130">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-130">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-131">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="221d5-131">extensionAttribute6</span></span>|<span data-ttu-id="221d5-132">String</span><span class="sxs-lookup"><span data-stu-id="221d5-132">String</span></span>| <span data-ttu-id="221d5-133">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-133">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-134">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="221d5-134">extensionAttribute7</span></span>|<span data-ttu-id="221d5-135">String</span><span class="sxs-lookup"><span data-stu-id="221d5-135">String</span></span>| <span data-ttu-id="221d5-136">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-136">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-137">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="221d5-137">extensionAttribute8</span></span>|<span data-ttu-id="221d5-138">String</span><span class="sxs-lookup"><span data-stu-id="221d5-138">String</span></span>| <span data-ttu-id="221d5-139">第八个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-139">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-140">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="221d5-140">extensionAttribute9</span></span>|<span data-ttu-id="221d5-141">String</span><span class="sxs-lookup"><span data-stu-id="221d5-141">String</span></span>| <span data-ttu-id="221d5-142">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-142">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-143">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="221d5-143">extensionAttribute10</span></span>|<span data-ttu-id="221d5-144">String</span><span class="sxs-lookup"><span data-stu-id="221d5-144">String</span></span>| <span data-ttu-id="221d5-145">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-145">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-146">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="221d5-146">extensionAttribute11</span></span>|<span data-ttu-id="221d5-147">String</span><span class="sxs-lookup"><span data-stu-id="221d5-147">String</span></span>| <span data-ttu-id="221d5-148">第十一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-148">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-149">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="221d5-149">extensionAttribute12</span></span>|<span data-ttu-id="221d5-150">String</span><span class="sxs-lookup"><span data-stu-id="221d5-150">String</span></span>| <span data-ttu-id="221d5-151">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-151">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-152">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="221d5-152">extensionAttribute13</span></span>|<span data-ttu-id="221d5-153">String</span><span class="sxs-lookup"><span data-stu-id="221d5-153">String</span></span>| <span data-ttu-id="221d5-154">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-154">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-155">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="221d5-155">extensionAttribute14</span></span>|<span data-ttu-id="221d5-156">String</span><span class="sxs-lookup"><span data-stu-id="221d5-156">String</span></span>| <span data-ttu-id="221d5-157">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-157">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="221d5-158">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="221d5-158">extensionAttribute15</span></span>|<span data-ttu-id="221d5-159">String</span><span class="sxs-lookup"><span data-stu-id="221d5-159">String</span></span>| <span data-ttu-id="221d5-160">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="221d5-160">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="221d5-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="221d5-161">JSON representation</span></span>

<span data-ttu-id="221d5-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="221d5-162">Here is a JSON representation of the resource</span></span>

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

