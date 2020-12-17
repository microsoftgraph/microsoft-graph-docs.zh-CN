---
title: userSource 资源类型
description: 保管人邮箱和 OneDrive for Business 网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 10184e053a0c62aaba6599f7d6f9bb6a33de8828
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706036"
---
# <a name="usersource-resource-type"></a><span data-ttu-id="29402-103">userSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="29402-103">userSource resource type</span></span>

<span data-ttu-id="29402-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29402-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29402-105">保管人邮箱 [和](custodian.md) OneDrive for Business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="29402-105">The container for a [custodian's](custodian.md) mailbox and OneDrive for Business site.</span></span>

## <a name="methods"></a><span data-ttu-id="29402-106">方法</span><span class="sxs-lookup"><span data-stu-id="29402-106">Methods</span></span>

|<span data-ttu-id="29402-107">方法</span><span class="sxs-lookup"><span data-stu-id="29402-107">Method</span></span>|<span data-ttu-id="29402-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="29402-108">Return type</span></span>|<span data-ttu-id="29402-109">说明</span><span class="sxs-lookup"><span data-stu-id="29402-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="29402-110">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="29402-110">List userSources</span></span>](../api/custodian-list-usersources.md)|<span data-ttu-id="29402-111">[userSource](../resources/usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29402-111">[userSource](../resources/usersource.md) collection</span></span>|<span data-ttu-id="29402-112">获取 **userSource 对象** 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="29402-112">Get a list of the **userSource** objects and their properties.</span></span>|
|[<span data-ttu-id="29402-113">创建 userSource</span><span class="sxs-lookup"><span data-stu-id="29402-113">Create userSource</span></span>](../api/custodian-post-usersources.md)|[<span data-ttu-id="29402-114">userSource</span><span class="sxs-lookup"><span data-stu-id="29402-114">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="29402-115">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="29402-115">Create a new **userSource** object.</span></span>|
|[<span data-ttu-id="29402-116">获取 userSource</span><span class="sxs-lookup"><span data-stu-id="29402-116">Get userSource</span></span>](../api/usersource-get.md)|[<span data-ttu-id="29402-117">userSource</span><span class="sxs-lookup"><span data-stu-id="29402-117">userSource</span></span>](../resources/usersource.md)|<span data-ttu-id="29402-118">读取 **userSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29402-118">Read the properties and relationships of a **userSource** object.</span></span>|
|[<span data-ttu-id="29402-119">删除 userSource</span><span class="sxs-lookup"><span data-stu-id="29402-119">Delete userSource</span></span>](../api/usersource-delete.md)|<span data-ttu-id="29402-120">无</span><span class="sxs-lookup"><span data-stu-id="29402-120">None</span></span>|<span data-ttu-id="29402-121">删除 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="29402-121">Delete a **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29402-122">属性</span><span class="sxs-lookup"><span data-stu-id="29402-122">Properties</span></span>

|<span data-ttu-id="29402-123">属性</span><span class="sxs-lookup"><span data-stu-id="29402-123">Property</span></span>|<span data-ttu-id="29402-124">类型</span><span class="sxs-lookup"><span data-stu-id="29402-124">Type</span></span>|<span data-ttu-id="29402-125">说明</span><span class="sxs-lookup"><span data-stu-id="29402-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29402-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="29402-126">createdBy</span></span>|[<span data-ttu-id="29402-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="29402-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="29402-128">创建 **userSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="29402-128">The user who created the **userSource**.</span></span>|
|<span data-ttu-id="29402-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="29402-129">createdDateTime</span></span>|<span data-ttu-id="29402-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29402-130">DateTimeOffset</span></span>|<span data-ttu-id="29402-131">创建 **userSource 的** 日期和时间</span><span class="sxs-lookup"><span data-stu-id="29402-131">The date and time the **userSource** was created</span></span>|
|<span data-ttu-id="29402-132">displayName</span><span class="sxs-lookup"><span data-stu-id="29402-132">displayName</span></span>|<span data-ttu-id="29402-133">字符串</span><span class="sxs-lookup"><span data-stu-id="29402-133">String</span></span>|<span data-ttu-id="29402-134">与显示名称和网站关联的邮箱。</span><span class="sxs-lookup"><span data-stu-id="29402-134">The display name associated with the mailbox and site.</span></span>|
|<span data-ttu-id="29402-135">email</span><span class="sxs-lookup"><span data-stu-id="29402-135">email</span></span>|<span data-ttu-id="29402-136">字符串</span><span class="sxs-lookup"><span data-stu-id="29402-136">String</span></span>|<span data-ttu-id="29402-137">用户邮箱的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="29402-137">Email address of the user's mailbox.</span></span>|
|<span data-ttu-id="29402-138">id</span><span class="sxs-lookup"><span data-stu-id="29402-138">id</span></span>|<span data-ttu-id="29402-139">字符串</span><span class="sxs-lookup"><span data-stu-id="29402-139">String</span></span>|<span data-ttu-id="29402-140">userSource 的ID。</span><span class="sxs-lookup"><span data-stu-id="29402-140">The ID of the **userSource**.</span></span> <span data-ttu-id="29402-141">这不是实际组的 ID</span><span class="sxs-lookup"><span data-stu-id="29402-141">This is not the ID of the actual group</span></span>|
|<span data-ttu-id="29402-142">includedSources</span><span class="sxs-lookup"><span data-stu-id="29402-142">includedSources</span></span>|<span data-ttu-id="29402-143">sourceType</span><span class="sxs-lookup"><span data-stu-id="29402-143">sourceType</span></span>|<span data-ttu-id="29402-144">指定此组中包含的源。</span><span class="sxs-lookup"><span data-stu-id="29402-144">Specifies which sources are included in this group.</span></span> <span data-ttu-id="29402-145">可取值为：`mailbox`、`site`。</span><span class="sxs-lookup"><span data-stu-id="29402-145">Possible values are: `mailbox`, `site`.</span></span>|

### <a name="sourcetype-values"></a><span data-ttu-id="29402-146">sourceType 值</span><span class="sxs-lookup"><span data-stu-id="29402-146">sourceType values</span></span>

<span data-ttu-id="29402-147">与用户相关的源类型。</span><span class="sxs-lookup"><span data-stu-id="29402-147">Types of source related to the user.</span></span> <span data-ttu-id="29402-148">默认情况下包括邮箱和网站。</span><span class="sxs-lookup"><span data-stu-id="29402-148">Includes mailbox and site by default.</span></span>

|<span data-ttu-id="29402-149">成员</span><span class="sxs-lookup"><span data-stu-id="29402-149">Member</span></span>|<span data-ttu-id="29402-150">说明</span><span class="sxs-lookup"><span data-stu-id="29402-150">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="29402-151">邮箱</span><span class="sxs-lookup"><span data-stu-id="29402-151">mailbox</span></span>|<span data-ttu-id="29402-152">表示邮箱。</span><span class="sxs-lookup"><span data-stu-id="29402-152">Represents a mailbox.</span></span>|
|<span data-ttu-id="29402-153">网站</span><span class="sxs-lookup"><span data-stu-id="29402-153">site</span></span>|<span data-ttu-id="29402-154">代表 OneDrive for Business 网站。</span><span class="sxs-lookup"><span data-stu-id="29402-154">Represents a OneDrive for Business site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29402-155">关系</span><span class="sxs-lookup"><span data-stu-id="29402-155">Relationships</span></span>

<span data-ttu-id="29402-156">无。</span><span class="sxs-lookup"><span data-stu-id="29402-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="29402-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29402-157">JSON representation</span></span>

<span data-ttu-id="29402-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29402-158">The following is a JSON representation of the resource.</span></span>
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
