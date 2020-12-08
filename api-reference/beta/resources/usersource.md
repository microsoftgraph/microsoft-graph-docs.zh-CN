---
title: userSource 资源类型
description: 保管人邮箱和 OneDrive for business 网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 2ce5448947bded580cc4896ba549d7cc6fab95f9
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597512"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="c5446-103">userSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5446-103">userSource resource type</span></span>

<span data-ttu-id="c5446-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5446-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5446-105">[保管人](custodian.md)邮箱和 OneDrive for business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="c5446-105">The container for a [custodian's](custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="c5446-106">方法</span><span class="sxs-lookup"><span data-stu-id="c5446-106">Methods</span></span>

|<span data-ttu-id="c5446-107">方法</span><span class="sxs-lookup"><span data-stu-id="c5446-107">Method</span></span>|<span data-ttu-id="c5446-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5446-108">Return type</span></span>|<span data-ttu-id="c5446-109">Description</span><span class="sxs-lookup"><span data-stu-id="c5446-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5446-110">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="c5446-110">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="c5446-111">[userSource](../resources/usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c5446-111">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="c5446-112">获取 **userSource** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c5446-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="c5446-113">创建 userSource</span><span class="sxs-lookup"><span data-stu-id="c5446-113">Create userSource</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="c5446-114">userSource</span><span class="sxs-lookup"><span data-stu-id="c5446-114">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="c5446-115">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="c5446-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="c5446-116">获取 userSource</span><span class="sxs-lookup"><span data-stu-id="c5446-116">Get userSource</span></span>](../api/usersource-get.md)|[<span data-ttu-id="c5446-117">userSource</span><span class="sxs-lookup"><span data-stu-id="c5446-117">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="c5446-118">读取 **userSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5446-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="c5446-119">删除 userSource</span><span class="sxs-lookup"><span data-stu-id="c5446-119">Delete userSource</span></span>](../api/usersource-delete.md)|<span data-ttu-id="c5446-120">无</span><span class="sxs-lookup"><span data-stu-id="c5446-120">None</span></span>|<span data-ttu-id="c5446-121">删除 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="c5446-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5446-122">属性</span><span class="sxs-lookup"><span data-stu-id="c5446-122">Properties</span></span>

|<span data-ttu-id="c5446-123">属性</span><span class="sxs-lookup"><span data-stu-id="c5446-123">Property</span></span>|<span data-ttu-id="c5446-124">类型</span><span class="sxs-lookup"><span data-stu-id="c5446-124">Type</span></span>|<span data-ttu-id="c5446-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5446-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5446-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="c5446-126">createdBy</span></span>|[<span data-ttu-id="c5446-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="c5446-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="c5446-128">创建 **userSource** 的用户。</span><span class="sxs-lookup"><span data-stu-id="c5446-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="c5446-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5446-129">createdDateTime</span></span>|<span data-ttu-id="c5446-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5446-130">DateTimeOffset</span></span>|<span data-ttu-id="c5446-131">美国 **userSource** erSource 的创建日期和时间</span><span class="sxs-lookup"><span data-stu-id="c5446-131">The date and time the us **userSource** erSource was created</span></span>|
|<span data-ttu-id="c5446-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c5446-132">displayName</span></span>|<span data-ttu-id="c5446-133">String</span><span class="sxs-lookup"><span data-stu-id="c5446-133">String</span></span>|<span data-ttu-id="c5446-134">与邮箱和网站关联的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c5446-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="c5446-135">email</span><span class="sxs-lookup"><span data-stu-id="c5446-135">email</span></span>|<span data-ttu-id="c5446-136">String</span><span class="sxs-lookup"><span data-stu-id="c5446-136">String</span></span>|<span data-ttu-id="c5446-137">用户邮箱的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c5446-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="c5446-138">id</span><span class="sxs-lookup"><span data-stu-id="c5446-138">id</span></span>|<span data-ttu-id="c5446-139">String</span><span class="sxs-lookup"><span data-stu-id="c5446-139">String</span></span>|<span data-ttu-id="c5446-140">**UserSource** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="c5446-140">The ID of the **userSource**.</span></span> <span data-ttu-id="c5446-141">这不是实际组的 ID</span><span class="sxs-lookup"><span data-stu-id="c5446-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="c5446-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="c5446-142">includedSources</span></span>|<span data-ttu-id="c5446-143">sourceType</span><span class="sxs-lookup"><span data-stu-id="c5446-143">sourceType</span></span>|<span data-ttu-id="c5446-144">指定要包含在此组中的源。</span><span class="sxs-lookup"><span data-stu-id="c5446-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="c5446-145">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="c5446-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="c5446-146">sourceType 值</span><span class="sxs-lookup"><span data-stu-id="c5446-146">sourceType values</span></span>

<span data-ttu-id="c5446-147">与用户相关的源的类型。</span><span class="sxs-lookup"><span data-stu-id="c5446-147">Types of source related to the user.</span></span> <span data-ttu-id="c5446-148">默认情况下包括邮箱和网站。</span><span class="sxs-lookup"><span data-stu-id="c5446-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="c5446-149">成员</span><span class="sxs-lookup"><span data-stu-id="c5446-149">Member</span></span>|<span data-ttu-id="c5446-150">说明</span><span class="sxs-lookup"><span data-stu-id="c5446-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="c5446-151">邮箱</span><span class="sxs-lookup"><span data-stu-id="c5446-151">mailbox</span></span>|<span data-ttu-id="c5446-152">代表一个邮箱。</span><span class="sxs-lookup"><span data-stu-id="c5446-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="c5446-153">网站</span><span class="sxs-lookup"><span data-stu-id="c5446-153">site</span></span>|<span data-ttu-id="c5446-154">表示 OneDrive for business 网站。</span><span class="sxs-lookup"><span data-stu-id="c5446-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5446-155">关系</span><span class="sxs-lookup"><span data-stu-id="c5446-155">Relationships</span></span>

<span data-ttu-id="c5446-156">无。</span><span class="sxs-lookup"><span data-stu-id="c5446-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5446-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5446-157">JSON representation</span></span>

<span data-ttu-id="c5446-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5446-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userSource",
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
