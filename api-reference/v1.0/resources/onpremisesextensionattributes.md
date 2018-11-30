---
title: onPremisesExtensionAttributes 资源类型
description: 用户实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。 仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。
ms.openlocfilehash: e5a56b5a846cf48cfc819b6d884689be10d6992e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009864"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="3717b-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="3717b-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="3717b-106">[用户](user.md)实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="3717b-107">此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。</span><span class="sxs-lookup"><span data-stu-id="3717b-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="3717b-108">仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。</span><span class="sxs-lookup"><span data-stu-id="3717b-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="3717b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3717b-109">Properties</span></span>
| <span data-ttu-id="3717b-110">属性</span><span class="sxs-lookup"><span data-stu-id="3717b-110">Property</span></span>     | <span data-ttu-id="3717b-111">类型</span><span class="sxs-lookup"><span data-stu-id="3717b-111">Type</span></span>   |<span data-ttu-id="3717b-112">说明</span><span class="sxs-lookup"><span data-stu-id="3717b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3717b-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="3717b-113">extensionAttribute1</span></span>|<span data-ttu-id="3717b-114">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-114">String</span></span>| <span data-ttu-id="3717b-115">第一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="3717b-116">extensionAttribute2</span></span>|<span data-ttu-id="3717b-117">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-117">String</span></span>| <span data-ttu-id="3717b-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="3717b-119">extensionAttribute3</span></span>|<span data-ttu-id="3717b-120">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-120">String</span></span>| <span data-ttu-id="3717b-121">第三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="3717b-122">extensionAttribute4</span></span>|<span data-ttu-id="3717b-123">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-123">String</span></span>| <span data-ttu-id="3717b-124">第四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="3717b-125">extensionAttribute5</span></span>|<span data-ttu-id="3717b-126">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-126">String</span></span>| <span data-ttu-id="3717b-127">第五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="3717b-128">extensionAttribute6</span></span>|<span data-ttu-id="3717b-129">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-129">String</span></span>| <span data-ttu-id="3717b-130">第六个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="3717b-131">extensionAttribute7</span></span>|<span data-ttu-id="3717b-132">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-132">String</span></span>| <span data-ttu-id="3717b-133">第七个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="3717b-134">extensionAttribute8</span></span>|<span data-ttu-id="3717b-135">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-135">String</span></span>| <span data-ttu-id="3717b-136">第八个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="3717b-137">extensionAttribute9</span></span>|<span data-ttu-id="3717b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-138">String</span></span>| <span data-ttu-id="3717b-139">第九个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="3717b-140">extensionAttribute10</span></span>|<span data-ttu-id="3717b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-141">String</span></span>| <span data-ttu-id="3717b-142">第十个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="3717b-143">extensionAttribute11</span></span>|<span data-ttu-id="3717b-144">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-144">String</span></span>| <span data-ttu-id="3717b-145">第十一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="3717b-146">extensionAttribute12</span></span>|<span data-ttu-id="3717b-147">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-147">String</span></span>| <span data-ttu-id="3717b-148">第十二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="3717b-149">extensionAttribute13</span></span>|<span data-ttu-id="3717b-150">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-150">String</span></span>| <span data-ttu-id="3717b-151">第十三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="3717b-152">extensionAttribute14</span></span>|<span data-ttu-id="3717b-153">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-153">String</span></span>| <span data-ttu-id="3717b-154">第十四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="3717b-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="3717b-155">extensionAttribute15</span></span>|<span data-ttu-id="3717b-156">字符串</span><span class="sxs-lookup"><span data-stu-id="3717b-156">String</span></span>| <span data-ttu-id="3717b-157">第十五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3717b-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3717b-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3717b-158">JSON representation</span></span>

<span data-ttu-id="3717b-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3717b-159">Here is a JSON representation of the resource</span></span>

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