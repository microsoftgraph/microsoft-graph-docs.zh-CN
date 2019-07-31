---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。 对于**onPremisesSyncEnabled**用户, 这组属性在本地 Active Directory 中使用并同步到 Azure AD, 并且是只读的。 对于仅限云的用户 (其中**onPremisesSyncEnabled**为 false), 可以在创建或更新期间设置这些属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: cbcb3d548a99d33e05768c765ab7a7e06981acc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966397"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="662bc-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="662bc-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="662bc-106">[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="662bc-107">对于**onPremisesSyncEnabled**用户, 这组属性在本地 Active Directory 中使用并同步到 Azure AD, 并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="662bc-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="662bc-108">对于仅限云的用户 (其中**onPremisesSyncEnabled**为 false), 可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="662bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="662bc-109">Properties</span></span>
| <span data-ttu-id="662bc-110">属性</span><span class="sxs-lookup"><span data-stu-id="662bc-110">Property</span></span>     | <span data-ttu-id="662bc-111">类型</span><span class="sxs-lookup"><span data-stu-id="662bc-111">Type</span></span>   |<span data-ttu-id="662bc-112">说明</span><span class="sxs-lookup"><span data-stu-id="662bc-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="662bc-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="662bc-113">extensionAttribute1</span></span>|<span data-ttu-id="662bc-114">String</span><span class="sxs-lookup"><span data-stu-id="662bc-114">String</span></span>| <span data-ttu-id="662bc-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="662bc-116">extensionAttribute2</span></span>|<span data-ttu-id="662bc-117">String</span><span class="sxs-lookup"><span data-stu-id="662bc-117">String</span></span>| <span data-ttu-id="662bc-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="662bc-119">extensionAttribute3</span></span>|<span data-ttu-id="662bc-120">String</span><span class="sxs-lookup"><span data-stu-id="662bc-120">String</span></span>| <span data-ttu-id="662bc-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="662bc-122">extensionAttribute4</span></span>|<span data-ttu-id="662bc-123">String</span><span class="sxs-lookup"><span data-stu-id="662bc-123">String</span></span>| <span data-ttu-id="662bc-124">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="662bc-125">extensionAttribute5</span></span>|<span data-ttu-id="662bc-126">String</span><span class="sxs-lookup"><span data-stu-id="662bc-126">String</span></span>| <span data-ttu-id="662bc-127">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="662bc-128">extensionAttribute6</span></span>|<span data-ttu-id="662bc-129">String</span><span class="sxs-lookup"><span data-stu-id="662bc-129">String</span></span>| <span data-ttu-id="662bc-130">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="662bc-131">extensionAttribute7</span></span>|<span data-ttu-id="662bc-132">String</span><span class="sxs-lookup"><span data-stu-id="662bc-132">String</span></span>| <span data-ttu-id="662bc-133">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="662bc-134">extensionAttribute8</span></span>|<span data-ttu-id="662bc-135">String</span><span class="sxs-lookup"><span data-stu-id="662bc-135">String</span></span>| <span data-ttu-id="662bc-136">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="662bc-137">extensionAttribute9</span></span>|<span data-ttu-id="662bc-138">String</span><span class="sxs-lookup"><span data-stu-id="662bc-138">String</span></span>| <span data-ttu-id="662bc-139">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="662bc-140">extensionAttribute10</span></span>|<span data-ttu-id="662bc-141">String</span><span class="sxs-lookup"><span data-stu-id="662bc-141">String</span></span>| <span data-ttu-id="662bc-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="662bc-143">extensionAttribute11</span></span>|<span data-ttu-id="662bc-144">String</span><span class="sxs-lookup"><span data-stu-id="662bc-144">String</span></span>| <span data-ttu-id="662bc-145">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="662bc-146">extensionAttribute12</span></span>|<span data-ttu-id="662bc-147">String</span><span class="sxs-lookup"><span data-stu-id="662bc-147">String</span></span>| <span data-ttu-id="662bc-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="662bc-149">extensionAttribute13</span></span>|<span data-ttu-id="662bc-150">String</span><span class="sxs-lookup"><span data-stu-id="662bc-150">String</span></span>| <span data-ttu-id="662bc-151">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="662bc-152">extensionAttribute14</span></span>|<span data-ttu-id="662bc-153">String</span><span class="sxs-lookup"><span data-stu-id="662bc-153">String</span></span>| <span data-ttu-id="662bc-154">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="662bc-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="662bc-155">extensionAttribute15</span></span>|<span data-ttu-id="662bc-156">String</span><span class="sxs-lookup"><span data-stu-id="662bc-156">String</span></span>| <span data-ttu-id="662bc-157">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="662bc-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="662bc-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="662bc-158">JSON representation</span></span>

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
