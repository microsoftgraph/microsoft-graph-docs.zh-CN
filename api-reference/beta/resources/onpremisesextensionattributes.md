---
title: onPremisesExtensionAttributes 资源类型
description: 用户实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。 此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。 仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。
ms.openlocfilehash: 547fc8ac19059611f5983a8b5ee0bd905f130f79
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046967"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="8b877-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b877-105">onPremisesExtensionAttributes resource type</span></span>

> <span data-ttu-id="8b877-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8b877-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b877-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8b877-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b877-108">[用户](user.md)实体的**onPremisesExtensionAttributes**属性包含 15 个自定义扩展特性的属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-108">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="8b877-109">此组属性是**onPremisesSyncEnabled**用户掌握了内部部署 Active Directory 中和同步到 Azure AD 和是只读的。</span><span class="sxs-lookup"><span data-stu-id="8b877-109">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="8b877-110">仅限云用户 （其中**onPremisesSyncEnabled**为 false），这些属性的创建过程中可以设置或更新。</span><span class="sxs-lookup"><span data-stu-id="8b877-110">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="8b877-111">属性</span><span class="sxs-lookup"><span data-stu-id="8b877-111">Properties</span></span>
| <span data-ttu-id="8b877-112">属性</span><span class="sxs-lookup"><span data-stu-id="8b877-112">Property</span></span>     | <span data-ttu-id="8b877-113">类型</span><span class="sxs-lookup"><span data-stu-id="8b877-113">Type</span></span>   |<span data-ttu-id="8b877-114">说明</span><span class="sxs-lookup"><span data-stu-id="8b877-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b877-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="8b877-115">extensionAttribute1</span></span>|<span data-ttu-id="8b877-116">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-116">String</span></span>| <span data-ttu-id="8b877-117">第一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="8b877-118">extensionAttribute2</span></span>|<span data-ttu-id="8b877-119">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-119">String</span></span>| <span data-ttu-id="8b877-120">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="8b877-121">extensionAttribute3</span></span>|<span data-ttu-id="8b877-122">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-122">String</span></span>| <span data-ttu-id="8b877-123">第三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="8b877-124">extensionAttribute4</span></span>|<span data-ttu-id="8b877-125">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-125">String</span></span>| <span data-ttu-id="8b877-126">第四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="8b877-127">extensionAttribute5</span></span>|<span data-ttu-id="8b877-128">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-128">String</span></span>| <span data-ttu-id="8b877-129">第五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="8b877-130">extensionAttribute6</span></span>|<span data-ttu-id="8b877-131">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-131">String</span></span>| <span data-ttu-id="8b877-132">第六个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="8b877-133">extensionAttribute7</span></span>|<span data-ttu-id="8b877-134">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-134">String</span></span>| <span data-ttu-id="8b877-135">第七个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="8b877-136">extensionAttribute8</span></span>|<span data-ttu-id="8b877-137">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-137">String</span></span>| <span data-ttu-id="8b877-138">第八个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="8b877-139">extensionAttribute9</span></span>|<span data-ttu-id="8b877-140">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-140">String</span></span>| <span data-ttu-id="8b877-141">第九个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="8b877-142">extensionAttribute10</span></span>|<span data-ttu-id="8b877-143">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-143">String</span></span>| <span data-ttu-id="8b877-144">第十个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="8b877-145">extensionAttribute11</span></span>|<span data-ttu-id="8b877-146">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-146">String</span></span>| <span data-ttu-id="8b877-147">第十一个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="8b877-148">extensionAttribute12</span></span>|<span data-ttu-id="8b877-149">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-149">String</span></span>| <span data-ttu-id="8b877-150">第十二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="8b877-151">extensionAttribute13</span></span>|<span data-ttu-id="8b877-152">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-152">String</span></span>| <span data-ttu-id="8b877-153">第十三个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="8b877-154">extensionAttribute14</span></span>|<span data-ttu-id="8b877-155">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-155">String</span></span>| <span data-ttu-id="8b877-156">第十四个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="8b877-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="8b877-157">extensionAttribute15</span></span>|<span data-ttu-id="8b877-158">字符串</span><span class="sxs-lookup"><span data-stu-id="8b877-158">String</span></span>| <span data-ttu-id="8b877-159">第十五个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8b877-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8b877-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b877-160">JSON representation</span></span>

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