---
title: onPremisesExtensionAttributes 资源类型
description: User 实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。 对于**onPremisesSyncEnabled**用户，这组属性在本地 Active Directory 中使用并同步到 Azure AD，并且是只读的。 对于仅限云的用户（其中**onPremisesSyncEnabled**为 false），可以在创建或更新期间设置这些属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: japere
ms.openlocfilehash: 06f1fb9fea5338a93c92a2bce2e31098046528bc
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200227"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="239ec-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="239ec-105">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="239ec-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="239ec-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="239ec-107">[User](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-107">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="239ec-108">对于**onPremisesSyncEnabled**用户，这组属性在本地 Active Directory 中使用并同步到 Azure AD，并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="239ec-108">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="239ec-109">对于仅限云的用户（其中**onPremisesSyncEnabled**为 false），可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-109">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="239ec-110">属性</span><span class="sxs-lookup"><span data-stu-id="239ec-110">Properties</span></span>
| <span data-ttu-id="239ec-111">属性</span><span class="sxs-lookup"><span data-stu-id="239ec-111">Property</span></span>     | <span data-ttu-id="239ec-112">类型</span><span class="sxs-lookup"><span data-stu-id="239ec-112">Type</span></span>   |<span data-ttu-id="239ec-113">说明</span><span class="sxs-lookup"><span data-stu-id="239ec-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="239ec-114">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="239ec-114">extensionAttribute1</span></span>|<span data-ttu-id="239ec-115">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-115">String</span></span>| <span data-ttu-id="239ec-116">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-116">First customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-117">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="239ec-117">extensionAttribute2</span></span>|<span data-ttu-id="239ec-118">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-118">String</span></span>| <span data-ttu-id="239ec-119">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-119">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-120">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="239ec-120">extensionAttribute3</span></span>|<span data-ttu-id="239ec-121">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-121">String</span></span>| <span data-ttu-id="239ec-122">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-122">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-123">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="239ec-123">extensionAttribute4</span></span>|<span data-ttu-id="239ec-124">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-124">String</span></span>| <span data-ttu-id="239ec-125">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-125">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-126">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="239ec-126">extensionAttribute5</span></span>|<span data-ttu-id="239ec-127">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-127">String</span></span>| <span data-ttu-id="239ec-128">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-128">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-129">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="239ec-129">extensionAttribute6</span></span>|<span data-ttu-id="239ec-130">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-130">String</span></span>| <span data-ttu-id="239ec-131">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-131">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-132">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="239ec-132">extensionAttribute7</span></span>|<span data-ttu-id="239ec-133">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-133">String</span></span>| <span data-ttu-id="239ec-134">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-134">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-135">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="239ec-135">extensionAttribute8</span></span>|<span data-ttu-id="239ec-136">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-136">String</span></span>| <span data-ttu-id="239ec-137">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-137">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-138">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="239ec-138">extensionAttribute9</span></span>|<span data-ttu-id="239ec-139">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-139">String</span></span>| <span data-ttu-id="239ec-140">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-140">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-141">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="239ec-141">extensionAttribute10</span></span>|<span data-ttu-id="239ec-142">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-142">String</span></span>| <span data-ttu-id="239ec-143">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-143">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-144">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="239ec-144">extensionAttribute11</span></span>|<span data-ttu-id="239ec-145">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-145">String</span></span>| <span data-ttu-id="239ec-146">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-146">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-147">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="239ec-147">extensionAttribute12</span></span>|<span data-ttu-id="239ec-148">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-148">String</span></span>| <span data-ttu-id="239ec-149">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-149">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-150">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="239ec-150">extensionAttribute13</span></span>|<span data-ttu-id="239ec-151">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-151">String</span></span>| <span data-ttu-id="239ec-152">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-152">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-153">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="239ec-153">extensionAttribute14</span></span>|<span data-ttu-id="239ec-154">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-154">String</span></span>| <span data-ttu-id="239ec-155">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-155">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="239ec-156">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="239ec-156">extensionAttribute15</span></span>|<span data-ttu-id="239ec-157">字符串</span><span class="sxs-lookup"><span data-stu-id="239ec-157">String</span></span>| <span data-ttu-id="239ec-158">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="239ec-158">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="239ec-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="239ec-159">JSON representation</span></span>

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
