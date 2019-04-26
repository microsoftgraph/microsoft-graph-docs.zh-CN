---
title: onPremisesExtensionAttributes 资源类型
description: user 实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。 对于**onPremisesSyncEnabled**用户, 这组属性在本地 Active Directory 中使用并同步到 Azure AD, 并且是只读的。 对于仅限云的用户 (其中**onPremisesSyncEnabled**为 false), 可以在创建或更新期间设置这些属性。
localization_priority: Normal
ms.openlocfilehash: f44f71fdcd86d2165289282568a2d7153ccc99b1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568877"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="44414-105">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="44414-105">onPremisesExtensionAttributes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44414-106">[user](user.md)实体的**onPremisesExtensionAttributes**属性包含十五个自定义扩展属性的属性。</span><span class="sxs-lookup"><span data-stu-id="44414-106">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="44414-107">对于**onPremisesSyncEnabled**用户, 这组属性在本地 Active Directory 中使用并同步到 Azure AD, 并且是只读的。</span><span class="sxs-lookup"><span data-stu-id="44414-107">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="44414-108">对于仅限云的用户 (其中**onPremisesSyncEnabled**为 false), 可以在创建或更新期间设置这些属性。</span><span class="sxs-lookup"><span data-stu-id="44414-108">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="44414-109">属性</span><span class="sxs-lookup"><span data-stu-id="44414-109">Properties</span></span>
| <span data-ttu-id="44414-110">属性</span><span class="sxs-lookup"><span data-stu-id="44414-110">Property</span></span>     | <span data-ttu-id="44414-111">类型</span><span class="sxs-lookup"><span data-stu-id="44414-111">Type</span></span>   |<span data-ttu-id="44414-112">说明</span><span class="sxs-lookup"><span data-stu-id="44414-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44414-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="44414-113">extensionAttribute1</span></span>|<span data-ttu-id="44414-114">String</span><span class="sxs-lookup"><span data-stu-id="44414-114">String</span></span>| <span data-ttu-id="44414-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="44414-116">extensionAttribute2</span></span>|<span data-ttu-id="44414-117">String</span><span class="sxs-lookup"><span data-stu-id="44414-117">String</span></span>| <span data-ttu-id="44414-118">第二个可自定义扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="44414-119">extensionAttribute3</span></span>|<span data-ttu-id="44414-120">String</span><span class="sxs-lookup"><span data-stu-id="44414-120">String</span></span>| <span data-ttu-id="44414-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="44414-122">extensionAttribute4</span></span>|<span data-ttu-id="44414-123">String</span><span class="sxs-lookup"><span data-stu-id="44414-123">String</span></span>| <span data-ttu-id="44414-124">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="44414-125">extensionAttribute5</span></span>|<span data-ttu-id="44414-126">String</span><span class="sxs-lookup"><span data-stu-id="44414-126">String</span></span>| <span data-ttu-id="44414-127">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="44414-128">extensionAttribute6</span></span>|<span data-ttu-id="44414-129">String</span><span class="sxs-lookup"><span data-stu-id="44414-129">String</span></span>| <span data-ttu-id="44414-130">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="44414-131">extensionAttribute7</span></span>|<span data-ttu-id="44414-132">String</span><span class="sxs-lookup"><span data-stu-id="44414-132">String</span></span>| <span data-ttu-id="44414-133">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="44414-134">extensionAttribute8</span></span>|<span data-ttu-id="44414-135">String</span><span class="sxs-lookup"><span data-stu-id="44414-135">String</span></span>| <span data-ttu-id="44414-136">第8个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="44414-137">extensionAttribute9</span></span>|<span data-ttu-id="44414-138">String</span><span class="sxs-lookup"><span data-stu-id="44414-138">String</span></span>| <span data-ttu-id="44414-139">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="44414-140">extensionAttribute10</span></span>|<span data-ttu-id="44414-141">String</span><span class="sxs-lookup"><span data-stu-id="44414-141">String</span></span>| <span data-ttu-id="44414-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="44414-143">extensionAttribute11</span></span>|<span data-ttu-id="44414-144">String</span><span class="sxs-lookup"><span data-stu-id="44414-144">String</span></span>| <span data-ttu-id="44414-145">第11个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="44414-146">extensionAttribute12</span></span>|<span data-ttu-id="44414-147">String</span><span class="sxs-lookup"><span data-stu-id="44414-147">String</span></span>| <span data-ttu-id="44414-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="44414-149">extensionAttribute13</span></span>|<span data-ttu-id="44414-150">String</span><span class="sxs-lookup"><span data-stu-id="44414-150">String</span></span>| <span data-ttu-id="44414-151">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="44414-152">extensionAttribute14</span></span>|<span data-ttu-id="44414-153">String</span><span class="sxs-lookup"><span data-stu-id="44414-153">String</span></span>| <span data-ttu-id="44414-154">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="44414-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="44414-155">extensionAttribute15</span></span>|<span data-ttu-id="44414-156">String</span><span class="sxs-lookup"><span data-stu-id="44414-156">String</span></span>| <span data-ttu-id="44414-157">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="44414-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44414-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44414-158">JSON representation</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesextensionattributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
