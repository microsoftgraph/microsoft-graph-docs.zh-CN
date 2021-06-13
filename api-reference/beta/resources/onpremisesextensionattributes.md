---
title: onPremisesExtensionAttributes 资源类型
description: user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 902ebfa8efe11613d6622d93ec0d39becc9e9bae
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912101"
---
# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="527df-103">onPremisesExtensionAttributes 资源类型</span><span class="sxs-lookup"><span data-stu-id="527df-103">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="527df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="527df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="527df-105">user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="527df-105">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="527df-106">对于 **onPremisesSyncEnabled** 用户，这组属性的颁发机构是同步到 Azure AD 且只读的本地 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="527df-106">For an **onPremisesSyncEnabled** user, the source of authority for this set of properties is the on-premises Active Directory which is synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="527df-107">对于仅云用户 (**onPremisesSyncEnabled**) ，可以在创建或更新期间设置 `false` [这些属性](../api/user-update.md)。 [](../api/user-post-users.md)</span><span class="sxs-lookup"><span data-stu-id="527df-107">For a cloud-only user (where **onPremisesSyncEnabled** is `false`), these properties may be set during [creation](../api/user-post-users.md) or [update](../api/user-update.md).</span></span>

> <span data-ttu-id="527df-108">**注意：** 这些扩展属性也称为自定义Exchange 1-15。</span><span class="sxs-lookup"><span data-stu-id="527df-108">**Note:** These extension attributes are also known as Exchange custom attributes 1-15.</span></span>


## <a name="properties"></a><span data-ttu-id="527df-109">属性</span><span class="sxs-lookup"><span data-stu-id="527df-109">Properties</span></span>
| <span data-ttu-id="527df-110">属性</span><span class="sxs-lookup"><span data-stu-id="527df-110">Property</span></span>     | <span data-ttu-id="527df-111">类型</span><span class="sxs-lookup"><span data-stu-id="527df-111">Type</span></span>   |<span data-ttu-id="527df-112">说明</span><span class="sxs-lookup"><span data-stu-id="527df-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="527df-113">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="527df-113">extensionAttribute1</span></span>|<span data-ttu-id="527df-114">String</span><span class="sxs-lookup"><span data-stu-id="527df-114">String</span></span>| <span data-ttu-id="527df-115">第一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-115">First customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-116">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="527df-116">extensionAttribute2</span></span>|<span data-ttu-id="527df-117">String</span><span class="sxs-lookup"><span data-stu-id="527df-117">String</span></span>| <span data-ttu-id="527df-118">第二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-118">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-119">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="527df-119">extensionAttribute3</span></span>|<span data-ttu-id="527df-120">String</span><span class="sxs-lookup"><span data-stu-id="527df-120">String</span></span>| <span data-ttu-id="527df-121">第三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-121">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-122">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="527df-122">extensionAttribute4</span></span>|<span data-ttu-id="527df-123">String</span><span class="sxs-lookup"><span data-stu-id="527df-123">String</span></span>| <span data-ttu-id="527df-124">第四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-124">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-125">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="527df-125">extensionAttribute5</span></span>|<span data-ttu-id="527df-126">String</span><span class="sxs-lookup"><span data-stu-id="527df-126">String</span></span>| <span data-ttu-id="527df-127">第五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-127">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-128">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="527df-128">extensionAttribute6</span></span>|<span data-ttu-id="527df-129">String</span><span class="sxs-lookup"><span data-stu-id="527df-129">String</span></span>| <span data-ttu-id="527df-130">第六个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-130">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-131">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="527df-131">extensionAttribute7</span></span>|<span data-ttu-id="527df-132">String</span><span class="sxs-lookup"><span data-stu-id="527df-132">String</span></span>| <span data-ttu-id="527df-133">第七个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-133">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-134">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="527df-134">extensionAttribute8</span></span>|<span data-ttu-id="527df-135">String</span><span class="sxs-lookup"><span data-stu-id="527df-135">String</span></span>| <span data-ttu-id="527df-136">第八个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-136">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-137">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="527df-137">extensionAttribute9</span></span>|<span data-ttu-id="527df-138">String</span><span class="sxs-lookup"><span data-stu-id="527df-138">String</span></span>| <span data-ttu-id="527df-139">第九个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-139">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-140">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="527df-140">extensionAttribute10</span></span>|<span data-ttu-id="527df-141">String</span><span class="sxs-lookup"><span data-stu-id="527df-141">String</span></span>| <span data-ttu-id="527df-142">第十个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-142">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-143">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="527df-143">extensionAttribute11</span></span>|<span data-ttu-id="527df-144">String</span><span class="sxs-lookup"><span data-stu-id="527df-144">String</span></span>| <span data-ttu-id="527df-145">第十一个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-145">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-146">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="527df-146">extensionAttribute12</span></span>|<span data-ttu-id="527df-147">String</span><span class="sxs-lookup"><span data-stu-id="527df-147">String</span></span>| <span data-ttu-id="527df-148">第十二个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-148">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-149">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="527df-149">extensionAttribute13</span></span>|<span data-ttu-id="527df-150">String</span><span class="sxs-lookup"><span data-stu-id="527df-150">String</span></span>| <span data-ttu-id="527df-151">第十三个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-151">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-152">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="527df-152">extensionAttribute14</span></span>|<span data-ttu-id="527df-153">String</span><span class="sxs-lookup"><span data-stu-id="527df-153">String</span></span>| <span data-ttu-id="527df-154">第十四个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-154">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="527df-155">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="527df-155">extensionAttribute15</span></span>|<span data-ttu-id="527df-156">String</span><span class="sxs-lookup"><span data-stu-id="527df-156">String</span></span>| <span data-ttu-id="527df-157">第十五个可自定义的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="527df-157">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="527df-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="527df-158">JSON representation</span></span>

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


