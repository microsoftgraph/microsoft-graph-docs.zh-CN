---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。 对于**onPremisesSyncEnabled**用户, 这组属性在本地 Active Directory 中使用并同步到 Azure AD, 并且是只读的。 对于仅限云的用户 (其中**onPremisesSyncEnabled**为 false), 可以在创建或更新期间设置这些属性。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c97e3bdc8f6c9a0a7558372288bfec4b9fb59593
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035754"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="7b95f-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b95f-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="7b95f-106">[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="7b95f-107">对于**onPremisesSyncEnabled**用户, 这组属性在本地 Active Directory 中使用并同步到 Azure AD, 并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="7b95f-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="7b95f-108">对于仅限云的用户 (其中**onPremisesSyncEnabled**为 false), 可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="7b95f-109">属性</span><span class="sxs-lookup"><span data-stu-id="7b95f-109">Properties</span></span>
| <span data-ttu-id="7b95f-110">属性</span><span class="sxs-lookup"><span data-stu-id="7b95f-110">Property</span></span>     | <span data-ttu-id="7b95f-111">类型</span><span class="sxs-lookup"><span data-stu-id="7b95f-111">Type</span></span>   |<span data-ttu-id="7b95f-112">说明</span><span class="sxs-lookup"><span data-stu-id="7b95f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b95f-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="7b95f-113">extensionAttribute1</span></span>|<span data-ttu-id="7b95f-114">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-114">String</span></span>| <span data-ttu-id="7b95f-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="7b95f-116">extensionAttribute2</span></span>|<span data-ttu-id="7b95f-117">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-117">String</span></span>| <span data-ttu-id="7b95f-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="7b95f-119">extensionAttribute3</span></span>|<span data-ttu-id="7b95f-120">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-120">String</span></span>| <span data-ttu-id="7b95f-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="7b95f-122">extensionAttribute4</span></span>|<span data-ttu-id="7b95f-123">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-123">String</span></span>| <span data-ttu-id="7b95f-124">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="7b95f-125">extensionAttribute5</span></span>|<span data-ttu-id="7b95f-126">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-126">String</span></span>| <span data-ttu-id="7b95f-127">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="7b95f-128">extensionAttribute6</span></span>|<span data-ttu-id="7b95f-129">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-129">String</span></span>| <span data-ttu-id="7b95f-130">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="7b95f-131">extensionAttribute7</span></span>|<span data-ttu-id="7b95f-132">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-132">String</span></span>| <span data-ttu-id="7b95f-133">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="7b95f-134">extensionAttribute8</span></span>|<span data-ttu-id="7b95f-135">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-135">String</span></span>| <span data-ttu-id="7b95f-136">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="7b95f-137">extensionAttribute9</span></span>|<span data-ttu-id="7b95f-138">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-138">String</span></span>| <span data-ttu-id="7b95f-139">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="7b95f-140">extensionAttribute10</span></span>|<span data-ttu-id="7b95f-141">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-141">String</span></span>| <span data-ttu-id="7b95f-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="7b95f-143">extensionAttribute11</span></span>|<span data-ttu-id="7b95f-144">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-144">String</span></span>| <span data-ttu-id="7b95f-145">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="7b95f-146">extensionAttribute12</span></span>|<span data-ttu-id="7b95f-147">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-147">String</span></span>| <span data-ttu-id="7b95f-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="7b95f-149">extensionAttribute13</span></span>|<span data-ttu-id="7b95f-150">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-150">String</span></span>| <span data-ttu-id="7b95f-151">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="7b95f-152">extensionAttribute14</span></span>|<span data-ttu-id="7b95f-153">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-153">String</span></span>| <span data-ttu-id="7b95f-154">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="7b95f-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="7b95f-155">extensionAttribute15</span></span>|<span data-ttu-id="7b95f-156">String</span><span class="sxs-lookup"><span data-stu-id="7b95f-156">String</span></span>| <span data-ttu-id="7b95f-157">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="7b95f-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7b95f-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b95f-158">JSON representation</span></span>

<span data-ttu-id="7b95f-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b95f-159">Here is a JSON representation of the resource</span></span>

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
