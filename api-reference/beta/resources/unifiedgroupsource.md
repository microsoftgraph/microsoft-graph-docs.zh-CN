---
title: unifiedGroupSource 资源类型
description: 管理员组的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 5fba2a994cda61f111739d98ea3a210c76ffeb23
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597589"
---
# <a name="unifiedgroupsource-resource-type"></a><span data-ttu-id="505c8-103">unifiedGroupSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="505c8-103">unifiedGroupSource resource type</span></span>

<span data-ttu-id="505c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="505c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="505c8-105">[管理员](custodian.md)组的容器。</span><span class="sxs-lookup"><span data-stu-id="505c8-105">The container for a [custodian's](custodian.md) group.</span></span>

## <a name="methods"></a><span data-ttu-id="505c8-106">方法</span><span class="sxs-lookup"><span data-stu-id="505c8-106">Methods</span></span>

|<span data-ttu-id="505c8-107">方法</span><span class="sxs-lookup"><span data-stu-id="505c8-107">Method</span></span>|<span data-ttu-id="505c8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="505c8-108">Return type</span></span>|<span data-ttu-id="505c8-109">Description</span><span class="sxs-lookup"><span data-stu-id="505c8-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="505c8-110">列出 unifiedGroupSources</span><span class="sxs-lookup"><span data-stu-id="505c8-110">List unifiedGroupSources</span></span>](../api/custodian-list-unifiedgroupsources.md)|<span data-ttu-id="505c8-111">[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="505c8-111">[unifiedGroupSource](../resources/unifiedgroupsource.md) collection</span></span>|<span data-ttu-id="505c8-112">获取 **unifiedGroupSource** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="505c8-112">Get a list of the **unifiedGroupSource** objects and their properties.</span></span>|
|[<span data-ttu-id="505c8-113">创建 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="505c8-113">Create unifiedGroupSource</span></span>](../api/custodian-post-unifiedgroupsources.md)|[<span data-ttu-id="505c8-114">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="505c8-114">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="505c8-115">创建新的 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="505c8-115">Create a new **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="505c8-116">获取 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="505c8-116">Get unifiedGroupSource</span></span>](../api/unifiedgroupsource-get.md)|[<span data-ttu-id="505c8-117">unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="505c8-117">unifiedGroupSource</span></span>](../resources/unifiedgroupsource.md)|<span data-ttu-id="505c8-118">读取 **unifiedGroupSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="505c8-118">Read the properties and relationships of a **unifiedGroupSource** object.</span></span>|
|[<span data-ttu-id="505c8-119">删除 unifiedGroupSource</span><span class="sxs-lookup"><span data-stu-id="505c8-119">Delete unifiedGroupSource</span></span>](../api/unifiedgroupsource-delete.md)|<span data-ttu-id="505c8-120">无</span><span class="sxs-lookup"><span data-stu-id="505c8-120">None</span></span>|<span data-ttu-id="505c8-121">删除 **unifiedGroupSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="505c8-121">Delete a **unifiedGroupSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="505c8-122">属性</span><span class="sxs-lookup"><span data-stu-id="505c8-122">Properties</span></span>

|<span data-ttu-id="505c8-123">属性</span><span class="sxs-lookup"><span data-stu-id="505c8-123">Property</span></span>|<span data-ttu-id="505c8-124">类型</span><span class="sxs-lookup"><span data-stu-id="505c8-124">Type</span></span>|<span data-ttu-id="505c8-125">说明</span><span class="sxs-lookup"><span data-stu-id="505c8-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="505c8-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="505c8-126">createdBy</span></span>|[<span data-ttu-id="505c8-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="505c8-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="505c8-128">创建 **unifiedGroupSource** 的用户。</span><span class="sxs-lookup"><span data-stu-id="505c8-128">The user who created the **unifiedGroupSource**.</span></span>|
|<span data-ttu-id="505c8-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="505c8-129">createdDateTime</span></span>|<span data-ttu-id="505c8-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="505c8-130">DateTimeOffset</span></span>|<span data-ttu-id="505c8-131">**UnifiedGroupSource** 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="505c8-131">The date and time the **unifiedGroupSource** was created.</span></span>|
|<span data-ttu-id="505c8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="505c8-132">displayName</span></span>|<span data-ttu-id="505c8-133">String</span><span class="sxs-lookup"><span data-stu-id="505c8-133">String</span></span>|<span data-ttu-id="505c8-134">统一组的显示名称-这是组的名称。</span><span class="sxs-lookup"><span data-stu-id="505c8-134">The display name of the unified group - This is the name of the group.</span></span>|
|<span data-ttu-id="505c8-135">id</span><span class="sxs-lookup"><span data-stu-id="505c8-135">id</span></span>|<span data-ttu-id="505c8-136">String</span><span class="sxs-lookup"><span data-stu-id="505c8-136">String</span></span>|<span data-ttu-id="505c8-137">**UnifiedGroupSource** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="505c8-137">The ID of the **unifiedGroupSource**.</span></span> <span data-ttu-id="505c8-138">这不是实际组的 ID。</span><span class="sxs-lookup"><span data-stu-id="505c8-138">This is not the ID of the actual group.</span></span>|
|<span data-ttu-id="505c8-139">includedSources</span><span class="sxs-lookup"><span data-stu-id="505c8-139">includedSources</span></span>|<span data-ttu-id="505c8-140">sourceType</span><span class="sxs-lookup"><span data-stu-id="505c8-140">sourceType</span></span>|<span data-ttu-id="505c8-141">指定要包含在此组中的源。</span><span class="sxs-lookup"><span data-stu-id="505c8-141">Specifies which sources are included in this group.</span></span> <span data-ttu-id="505c8-142">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="505c8-142">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="505c8-143">sourceType 值</span><span class="sxs-lookup"><span data-stu-id="505c8-143">sourceType values</span></span>

<span data-ttu-id="505c8-144">与用户相关的源的类型。</span><span class="sxs-lookup"><span data-stu-id="505c8-144">Types of source related to the user.</span></span> <span data-ttu-id="505c8-145">默认情况下包括邮箱和网站。</span><span class="sxs-lookup"><span data-stu-id="505c8-145">Includes mailbox and site both by default.</span></span>

|<span data-ttu-id="505c8-146">成员</span><span class="sxs-lookup"><span data-stu-id="505c8-146">Member</span></span>|<span data-ttu-id="505c8-147">说明</span><span class="sxs-lookup"><span data-stu-id="505c8-147">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="505c8-148">邮箱</span><span class="sxs-lookup"><span data-stu-id="505c8-148">mailbox</span></span>|<span data-ttu-id="505c8-149">代表一个邮箱。</span><span class="sxs-lookup"><span data-stu-id="505c8-149">Represents a mailbox.</span></span>|
|<span data-ttu-id="505c8-150">网站</span><span class="sxs-lookup"><span data-stu-id="505c8-150">site</span></span>|<span data-ttu-id="505c8-151">表示 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="505c8-151">Represents a SharePoint site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="505c8-152">关系</span><span class="sxs-lookup"><span data-stu-id="505c8-152">Relationships</span></span>

|<span data-ttu-id="505c8-153">关系</span><span class="sxs-lookup"><span data-stu-id="505c8-153">Relationship</span></span>|<span data-ttu-id="505c8-154">类型</span><span class="sxs-lookup"><span data-stu-id="505c8-154">Type</span></span>|<span data-ttu-id="505c8-155">Description</span><span class="sxs-lookup"><span data-stu-id="505c8-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="505c8-156">group</span><span class="sxs-lookup"><span data-stu-id="505c8-156">group</span></span>|[<span data-ttu-id="505c8-157">组</span><span class="sxs-lookup"><span data-stu-id="505c8-157">group</span></span>](../resources/group.md)|<span data-ttu-id="505c8-158">与 **unifiedGroupSource** 相关联的组。</span><span class="sxs-lookup"><span data-stu-id="505c8-158">The group associated with the **unifiedGroupSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="505c8-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="505c8-159">JSON representation</span></span>

<span data-ttu-id="505c8-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="505c8-160">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedGroupSource",
  "baseType": "microsoft.graph.dataSource",
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
