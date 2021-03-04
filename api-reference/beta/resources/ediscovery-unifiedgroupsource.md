---
title: unifiedGroupSource 资源类型
description: 保管人组容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b6d1b1d1a7d3abee2516e170fcead20c73235f1f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446651"
---
# <a name="unifiedgroupsource-resource-type"></a><span data-ttu-id="8a03d-103">unifiedGroupSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a03d-103">unifiedGroupSource resource type</span></span>

<span data-ttu-id="8a03d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8a03d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a03d-105">保管人 [组的容器](ediscovery-custodian.md) 。</span><span class="sxs-lookup"><span data-stu-id="8a03d-105">The container for a [custodian's](ediscovery-custodian.md) group.</span></span>

## <a name="methods"></a><span data-ttu-id="8a03d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8a03d-106">Methods</span></span>

|<span data-ttu-id="8a03d-107">方法</span><span class="sxs-lookup"><span data-stu-id="8a03d-107">Method</span></span>|<span data-ttu-id="8a03d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a03d-108">Return type</span></span>|<span data-ttu-id="8a03d-109">说明</span><span class="sxs-lookup"><span data-stu-id="8a03d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a03d-110">列出 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="8a03d-110">List unifiedGroupSources</span></span>](../api/ediscovery-custodian-list-unifiedgroupsources.md)|<span data-ttu-id="8a03d-111">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a03d-111">[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="8a03d-112">获取 **unifiedGroupSource** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="8a03d-112">Get a list of the **unifiedGroupSource** objects and their properties.</span></span>|
|[<span data-ttu-id="8a03d-113">创建 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="8a03d-113">Create unifiedGroupSource</span></span>](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="8a03d-114">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="8a03d-114">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="8a03d-115">创建新的 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="8a03d-115">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="8a03d-116">获取 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="8a03d-116">Get unifiedGroupSource</span></span>](../api/ediscovery-unifiedgroupsource-get.md)|[<span data-ttu-id="8a03d-117">microsoft.graph.ediscovery.unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="8a03d-117">microsoft.graph.ediscovery.unifiedGroupSource</span></span>](../resources/ediscovery-unifiedgroupsource.md)|<span data-ttu-id="8a03d-118">读取 **unifiedGroupSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8a03d-118">Read the properties and relationships of a **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="8a03d-119">删除 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="8a03d-119">Delete unifiedGroupSource</span></span>](../api/ediscovery-unifiedgroupsource-delete.md)|<span data-ttu-id="8a03d-120">无</span><span class="sxs-lookup"><span data-stu-id="8a03d-120">None</span></span>|<span data-ttu-id="8a03d-121">删除 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="8a03d-121">Delete a **unifiedGroupSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a03d-122">属性</span><span class="sxs-lookup"><span data-stu-id="8a03d-122">Properties</span></span>

|<span data-ttu-id="8a03d-123">属性</span><span class="sxs-lookup"><span data-stu-id="8a03d-123">Property</span></span>|<span data-ttu-id="8a03d-124">类型</span><span class="sxs-lookup"><span data-stu-id="8a03d-124">Type</span></span>|<span data-ttu-id="8a03d-125">说明</span><span class="sxs-lookup"><span data-stu-id="8a03d-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a03d-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="8a03d-126">createdBy</span></span>|[<span data-ttu-id="8a03d-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="8a03d-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="8a03d-128">创建 **unifiedGroupSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="8a03d-128">The user who created the **unifiedGroupSource**.</span></span>|
|<span data-ttu-id="8a03d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a03d-129">createdDateTime</span></span>|<span data-ttu-id="8a03d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a03d-130">DateTimeOffset</span></span>|<span data-ttu-id="8a03d-131">创建 **unifiedGroupSource 的** 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8a03d-131">The date and time the **unifiedGroupSource** was created.</span></span>|
|<span data-ttu-id="8a03d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8a03d-132">displayName</span></span>|<span data-ttu-id="8a03d-133">String</span><span class="sxs-lookup"><span data-stu-id="8a03d-133">String</span></span>|<span data-ttu-id="8a03d-134">统显示名称的名称 - 这是组的名称。</span><span class="sxs-lookup"><span data-stu-id="8a03d-134">The display name of the unified group - This is the name of the group.</span></span>|
|<span data-ttu-id="8a03d-135">id</span><span class="sxs-lookup"><span data-stu-id="8a03d-135">id</span></span>|<span data-ttu-id="8a03d-136">String</span><span class="sxs-lookup"><span data-stu-id="8a03d-136">String</span></span>|<span data-ttu-id="8a03d-137">**unifiedGroupSource** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a03d-137">The ID of the **unifiedGroupSource**.</span></span> <span data-ttu-id="8a03d-138">这不是实际组的 ID。</span><span class="sxs-lookup"><span data-stu-id="8a03d-138">This is not the ID of the actual group.</span></span>|
|<span data-ttu-id="8a03d-139">includedSources</span><span class="sxs-lookup"><span data-stu-id="8a03d-139">includedSources</span></span>|<span data-ttu-id="8a03d-140">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="8a03d-140">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="8a03d-141">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="8a03d-141">Specifies which sources are included in this group.</span></span> <span data-ttu-id="8a03d-142">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="8a03d-142">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="8a03d-143">sourceType 值</span><span class="sxs-lookup"><span data-stu-id="8a03d-143">sourceType values</span></span>

<span data-ttu-id="8a03d-144">与用户相关的源类型。</span><span class="sxs-lookup"><span data-stu-id="8a03d-144">Types of source related to the user.</span></span> <span data-ttu-id="8a03d-145">默认情况下包括邮箱和网站。</span><span class="sxs-lookup"><span data-stu-id="8a03d-145">Includes mailbox and site both by default.</span></span>

|<span data-ttu-id="8a03d-146">成员</span><span class="sxs-lookup"><span data-stu-id="8a03d-146">Member</span></span>|<span data-ttu-id="8a03d-147">说明</span><span class="sxs-lookup"><span data-stu-id="8a03d-147">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="8a03d-148">邮箱</span><span class="sxs-lookup"><span data-stu-id="8a03d-148">mailbox</span></span>|<span data-ttu-id="8a03d-149">表示邮箱。</span><span class="sxs-lookup"><span data-stu-id="8a03d-149">Represents a mailbox.</span></span>|
|<span data-ttu-id="8a03d-150">网站</span><span class="sxs-lookup"><span data-stu-id="8a03d-150">site</span></span>|<span data-ttu-id="8a03d-151">表示 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="8a03d-151">Represents a SharePoint site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a03d-152">关系</span><span class="sxs-lookup"><span data-stu-id="8a03d-152">Relationships</span></span>

|<span data-ttu-id="8a03d-153">关系</span><span class="sxs-lookup"><span data-stu-id="8a03d-153">Relationship</span></span>|<span data-ttu-id="8a03d-154">类型</span><span class="sxs-lookup"><span data-stu-id="8a03d-154">Type</span></span>|<span data-ttu-id="8a03d-155">说明</span><span class="sxs-lookup"><span data-stu-id="8a03d-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a03d-156">group</span><span class="sxs-lookup"><span data-stu-id="8a03d-156">group</span></span>|[<span data-ttu-id="8a03d-157">组</span><span class="sxs-lookup"><span data-stu-id="8a03d-157">group</span></span>](../resources/group.md)|<span data-ttu-id="8a03d-158">与 **unifiedGroupSource** 关联的组。</span><span class="sxs-lookup"><span data-stu-id="8a03d-158">The group associated with the **unifiedGroupSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a03d-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a03d-159">JSON representation</span></span>

<span data-ttu-id="8a03d-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a03d-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/unifiedGroupSources",
    "value": [
        {
            "displayName": "Developers group",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "33434233-3030-3739-3043-393039324633",
            "includedSources": "mailbox,site",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
