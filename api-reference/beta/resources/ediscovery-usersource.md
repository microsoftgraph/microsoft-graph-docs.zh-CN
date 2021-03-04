---
title: userSource 资源类型
description: 保管人邮箱和 OneDrive for Business 网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: f0d98ac894d3d60bed2bb249ef9daec707f6f7ba
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446650"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="a003d-103">userSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a003d-103">userSource resource type</span></span>

<span data-ttu-id="a003d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="a003d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a003d-105">保管人邮箱 [和](ediscovery-custodian.md) OneDrive for Business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="a003d-105">The container for a [custodian's](ediscovery-custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="a003d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a003d-106">Methods</span></span>

|<span data-ttu-id="a003d-107">方法</span><span class="sxs-lookup"><span data-stu-id="a003d-107">Method</span></span>|<span data-ttu-id="a003d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a003d-108">Return type</span></span>|<span data-ttu-id="a003d-109">说明</span><span class="sxs-lookup"><span data-stu-id="a003d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a003d-110">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="a003d-110">List userSources</span></span>](../api/ediscovery-custodian-list-usersources.md)|<span data-ttu-id="a003d-111">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a003d-111">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>|<span data-ttu-id="a003d-112">获取 **userSource 对象** 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="a003d-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="a003d-113">创建 userSource</span><span class="sxs-lookup"><span data-stu-id="a003d-113">Create userSource</span></span>](../api/ediscovery-custodian-post-usersources.md)|[<span data-ttu-id="a003d-114">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="a003d-114">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="a003d-115">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="a003d-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="a003d-116">获取 userSource</span><span class="sxs-lookup"><span data-stu-id="a003d-116">Get userSource</span></span>](../api/ediscovery-usersource-get.md)|[<span data-ttu-id="a003d-117">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="a003d-117">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="a003d-118">读取 **userSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a003d-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="a003d-119">删除 userSource</span><span class="sxs-lookup"><span data-stu-id="a003d-119">Delete userSource</span></span>](../api/ediscovery-usersource-delete.md)|<span data-ttu-id="a003d-120">无</span><span class="sxs-lookup"><span data-stu-id="a003d-120">None</span></span>|<span data-ttu-id="a003d-121">删除 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="a003d-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a003d-122">属性</span><span class="sxs-lookup"><span data-stu-id="a003d-122">Properties</span></span>

|<span data-ttu-id="a003d-123">属性</span><span class="sxs-lookup"><span data-stu-id="a003d-123">Property</span></span>|<span data-ttu-id="a003d-124">类型</span><span class="sxs-lookup"><span data-stu-id="a003d-124">Type</span></span>|<span data-ttu-id="a003d-125">说明</span><span class="sxs-lookup"><span data-stu-id="a003d-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a003d-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="a003d-126">createdBy</span></span>|[<span data-ttu-id="a003d-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="a003d-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a003d-128">创建 **userSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="a003d-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="a003d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a003d-129">createdDateTime</span></span>|<span data-ttu-id="a003d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a003d-130">DateTimeOffset</span></span>|<span data-ttu-id="a003d-131">创建 **userSource** 的日期和时间</span><span class="sxs-lookup"><span data-stu-id="a003d-131">The date and time the **userSource** was created</span></span>|
|<span data-ttu-id="a003d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a003d-132">displayName</span></span>|<span data-ttu-id="a003d-133">String</span><span class="sxs-lookup"><span data-stu-id="a003d-133">String</span></span>|<span data-ttu-id="a003d-134">与显示名称和网站关联的邮箱。</span><span class="sxs-lookup"><span data-stu-id="a003d-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="a003d-135">email</span><span class="sxs-lookup"><span data-stu-id="a003d-135">email</span></span>|<span data-ttu-id="a003d-136">String</span><span class="sxs-lookup"><span data-stu-id="a003d-136">String</span></span>|<span data-ttu-id="a003d-137">用户邮箱的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="a003d-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="a003d-138">id</span><span class="sxs-lookup"><span data-stu-id="a003d-138">id</span></span>|<span data-ttu-id="a003d-139">String</span><span class="sxs-lookup"><span data-stu-id="a003d-139">String</span></span>|<span data-ttu-id="a003d-140">userSource 的ID。</span><span class="sxs-lookup"><span data-stu-id="a003d-140">The ID of the **userSource**.</span></span> <span data-ttu-id="a003d-141">这不是实际组的 ID</span><span class="sxs-lookup"><span data-stu-id="a003d-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="a003d-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="a003d-142">includedSources</span></span>|<span data-ttu-id="a003d-143">microsoft.graph.ediscovery.sourceType</span><span class="sxs-lookup"><span data-stu-id="a003d-143">microsoft.graph.ediscovery.sourceType</span></span>|<span data-ttu-id="a003d-144">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="a003d-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="a003d-145">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="a003d-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="a003d-146">sourceType 值</span><span class="sxs-lookup"><span data-stu-id="a003d-146">sourceType values</span></span>

<span data-ttu-id="a003d-147">与用户相关的源类型。</span><span class="sxs-lookup"><span data-stu-id="a003d-147">Types of source related to the user.</span></span> <span data-ttu-id="a003d-148">默认情况下包括邮箱和网站。</span><span class="sxs-lookup"><span data-stu-id="a003d-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="a003d-149">成员</span><span class="sxs-lookup"><span data-stu-id="a003d-149">Member</span></span>|<span data-ttu-id="a003d-150">说明</span><span class="sxs-lookup"><span data-stu-id="a003d-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="a003d-151">邮箱</span><span class="sxs-lookup"><span data-stu-id="a003d-151">mailbox</span></span>|<span data-ttu-id="a003d-152">表示邮箱。</span><span class="sxs-lookup"><span data-stu-id="a003d-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="a003d-153">网站</span><span class="sxs-lookup"><span data-stu-id="a003d-153">site</span></span>|<span data-ttu-id="a003d-154">代表 OneDrive for Business 网站。</span><span class="sxs-lookup"><span data-stu-id="a003d-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a003d-155">关系</span><span class="sxs-lookup"><span data-stu-id="a003d-155">Relationships</span></span>

<span data-ttu-id="a003d-156">无。</span><span class="sxs-lookup"><span data-stu-id="a003d-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a003d-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a003d-157">JSON representation</span></span>

<span data-ttu-id="a003d-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a003d-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.userSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.userSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "email": "String",
  "includedSources": "String"
}
```
