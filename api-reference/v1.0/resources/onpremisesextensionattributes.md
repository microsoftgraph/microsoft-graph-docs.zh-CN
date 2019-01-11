---
title: onPremisesExtensionAttributes 资源类型
description: 用户实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。 仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。
localization_priority: Normal
ms.openlocfilehash: c0cb765efe9e94c8254e45eaa9d55bc16382f6d2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824743"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="f7f03-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7f03-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="f7f03-106">[用户](user.md)实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="f7f03-107">此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。</span><span class="sxs-lookup"><span data-stu-id="f7f03-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="f7f03-108">仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。</span><span class="sxs-lookup"><span data-stu-id="f7f03-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="f7f03-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7f03-109">Properties</span></span>
| <span data-ttu-id="f7f03-110">属性</span><span class="sxs-lookup"><span data-stu-id="f7f03-110">Property</span></span>     | <span data-ttu-id="f7f03-111">类型</span><span class="sxs-lookup"><span data-stu-id="f7f03-111">Type</span></span>   |<span data-ttu-id="f7f03-112">Description</span><span class="sxs-lookup"><span data-stu-id="f7f03-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7f03-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="f7f03-113">extensionAttribute1</span></span>|<span data-ttu-id="f7f03-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-114">String</span></span>| <span data-ttu-id="f7f03-115">第一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="f7f03-116">extensionAttribute2</span></span>|<span data-ttu-id="f7f03-117">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-117">String</span></span>| <span data-ttu-id="f7f03-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="f7f03-119">extensionAttribute3</span></span>|<span data-ttu-id="f7f03-120">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-120">String</span></span>| <span data-ttu-id="f7f03-121">第三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="f7f03-122">extensionAttribute4</span></span>|<span data-ttu-id="f7f03-123">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-123">String</span></span>| <span data-ttu-id="f7f03-124">第四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="f7f03-125">extensionAttribute5</span></span>|<span data-ttu-id="f7f03-126">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-126">String</span></span>| <span data-ttu-id="f7f03-127">第五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="f7f03-128">extensionAttribute6</span></span>|<span data-ttu-id="f7f03-129">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-129">String</span></span>| <span data-ttu-id="f7f03-130">第六个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="f7f03-131">extensionAttribute7</span></span>|<span data-ttu-id="f7f03-132">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-132">String</span></span>| <span data-ttu-id="f7f03-133">第七个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="f7f03-134">extensionAttribute8</span></span>|<span data-ttu-id="f7f03-135">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-135">String</span></span>| <span data-ttu-id="f7f03-136">第八个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="f7f03-137">extensionAttribute9</span></span>|<span data-ttu-id="f7f03-138">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-138">String</span></span>| <span data-ttu-id="f7f03-139">第九个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="f7f03-140">extensionAttribute10</span></span>|<span data-ttu-id="f7f03-141">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-141">String</span></span>| <span data-ttu-id="f7f03-142">第十个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="f7f03-143">extensionAttribute11</span></span>|<span data-ttu-id="f7f03-144">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-144">String</span></span>| <span data-ttu-id="f7f03-145">第十一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="f7f03-146">extensionAttribute12</span></span>|<span data-ttu-id="f7f03-147">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-147">String</span></span>| <span data-ttu-id="f7f03-148">第十二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="f7f03-149">extensionAttribute13</span></span>|<span data-ttu-id="f7f03-150">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-150">String</span></span>| <span data-ttu-id="f7f03-151">第十三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="f7f03-152">extensionAttribute14</span></span>|<span data-ttu-id="f7f03-153">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-153">String</span></span>| <span data-ttu-id="f7f03-154">第十四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="f7f03-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="f7f03-155">extensionAttribute15</span></span>|<span data-ttu-id="f7f03-156">字符串</span><span class="sxs-lookup"><span data-stu-id="f7f03-156">String</span></span>| <span data-ttu-id="f7f03-157">第十五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f7f03-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7f03-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7f03-158">JSON representation</span></span>

<span data-ttu-id="f7f03-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7f03-159">Here is a JSON representation of the resource</span></span>

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
