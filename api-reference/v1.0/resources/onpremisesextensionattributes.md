---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。 对于**onPremisesSyncEnabled**用户，这组属性在本地 Active Directory 中使用并同步到 Azure AD，并且是只读的。 对于仅限云的用户（其中**onPremisesSyncEnabled**为 false），可以在创建或更新期间设置这些属性。
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 84929229c18b905ff66b4a1bbbbf765771180a06
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864089"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="1070a-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="1070a-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="1070a-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1070a-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1070a-107">[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="1070a-108">对于**onPremisesSyncEnabled**用户，此属性集的权威来源是同步到 Azure AD 的本地 Active Directory，并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="1070a-108">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="1070a-109">对于仅限云的用户（其中**onPremisesSyncEnabled**为 false），可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>

> <span data-ttu-id="1070a-110">**注意：** 这些扩展属性也称为 Exchange 自定义属性1-15。</span><span class="sxs-lookup"><span data-stu-id="1070a-110">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>

## <a name="properties"></a><span data-ttu-id="1070a-111">属性</span><span class="sxs-lookup"><span data-stu-id="1070a-111">Properties</span></span>
| <span data-ttu-id="1070a-112">属性</span><span class="sxs-lookup"><span data-stu-id="1070a-112">Property</span></span>     | <span data-ttu-id="1070a-113">类型</span><span class="sxs-lookup"><span data-stu-id="1070a-113">Type</span></span>   |<span data-ttu-id="1070a-114">说明</span><span class="sxs-lookup"><span data-stu-id="1070a-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1070a-115">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="1070a-115">extensionAttribute1</span></span>|<span data-ttu-id="1070a-116">String</span><span class="sxs-lookup"><span data-stu-id="1070a-116">String</span></span>| <span data-ttu-id="1070a-117">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-117">First customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-118">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="1070a-118">extensionAttribute2</span></span>|<span data-ttu-id="1070a-119">String</span><span class="sxs-lookup"><span data-stu-id="1070a-119">String</span></span>| <span data-ttu-id="1070a-120">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-120">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-121">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="1070a-121">extensionAttribute3</span></span>|<span data-ttu-id="1070a-122">String</span><span class="sxs-lookup"><span data-stu-id="1070a-122">String</span></span>| <span data-ttu-id="1070a-123">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-123">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-124">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="1070a-124">extensionAttribute4</span></span>|<span data-ttu-id="1070a-125">String</span><span class="sxs-lookup"><span data-stu-id="1070a-125">String</span></span>| <span data-ttu-id="1070a-126">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-126">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-127">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="1070a-127">extensionAttribute5</span></span>|<span data-ttu-id="1070a-128">String</span><span class="sxs-lookup"><span data-stu-id="1070a-128">String</span></span>| <span data-ttu-id="1070a-129">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-129">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-130">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="1070a-130">extensionAttribute6</span></span>|<span data-ttu-id="1070a-131">String</span><span class="sxs-lookup"><span data-stu-id="1070a-131">String</span></span>| <span data-ttu-id="1070a-132">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-132">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-133">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="1070a-133">extensionAttribute7</span></span>|<span data-ttu-id="1070a-134">String</span><span class="sxs-lookup"><span data-stu-id="1070a-134">String</span></span>| <span data-ttu-id="1070a-135">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-135">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-136">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="1070a-136">extensionAttribute8</span></span>|<span data-ttu-id="1070a-137">String</span><span class="sxs-lookup"><span data-stu-id="1070a-137">String</span></span>| <span data-ttu-id="1070a-138">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-138">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-139">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="1070a-139">extensionAttribute9</span></span>|<span data-ttu-id="1070a-140">String</span><span class="sxs-lookup"><span data-stu-id="1070a-140">String</span></span>| <span data-ttu-id="1070a-141">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-141">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-142">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="1070a-142">extensionAttribute10</span></span>|<span data-ttu-id="1070a-143">String</span><span class="sxs-lookup"><span data-stu-id="1070a-143">String</span></span>| <span data-ttu-id="1070a-144">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-144">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-145">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="1070a-145">extensionAttribute11</span></span>|<span data-ttu-id="1070a-146">String</span><span class="sxs-lookup"><span data-stu-id="1070a-146">String</span></span>| <span data-ttu-id="1070a-147">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-147">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-148">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="1070a-148">extensionAttribute12</span></span>|<span data-ttu-id="1070a-149">String</span><span class="sxs-lookup"><span data-stu-id="1070a-149">String</span></span>| <span data-ttu-id="1070a-150">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-150">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-151">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="1070a-151">extensionAttribute13</span></span>|<span data-ttu-id="1070a-152">String</span><span class="sxs-lookup"><span data-stu-id="1070a-152">String</span></span>| <span data-ttu-id="1070a-153">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-153">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-154">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="1070a-154">extensionAttribute14</span></span>|<span data-ttu-id="1070a-155">String</span><span class="sxs-lookup"><span data-stu-id="1070a-155">String</span></span>| <span data-ttu-id="1070a-156">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-156">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="1070a-157">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="1070a-157">extensionAttribute15</span></span>|<span data-ttu-id="1070a-158">String</span><span class="sxs-lookup"><span data-stu-id="1070a-158">String</span></span>| <span data-ttu-id="1070a-159">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1070a-159">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1070a-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1070a-160">JSON representation</span></span>

<span data-ttu-id="1070a-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1070a-161">Here is a JSON representation of the resource</span></span>

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
