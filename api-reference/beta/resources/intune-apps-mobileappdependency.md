---
title: mobileAppDependency 资源类型
description: 描述两个移动应用程序之间的依赖关系类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8e6bdcd9cf5903d07fb858103bd3620e9a187da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161563"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="3e8f9-103">mobileAppDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="3e8f9-103">mobileAppDependency resource type</span></span>

<span data-ttu-id="3e8f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e8f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e8f9-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e8f9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e8f9-107">描述两个移动应用程序之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-107">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="3e8f9-108">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="3e8f9-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3e8f9-109">方法</span><span class="sxs-lookup"><span data-stu-id="3e8f9-109">Methods</span></span>
|<span data-ttu-id="3e8f9-110">方法</span><span class="sxs-lookup"><span data-stu-id="3e8f9-110">Method</span></span>|<span data-ttu-id="3e8f9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e8f9-111">Return Type</span></span>|<span data-ttu-id="3e8f9-112">说明</span><span class="sxs-lookup"><span data-stu-id="3e8f9-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e8f9-113">列出 mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="3e8f9-113">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="3e8f9-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e8f9-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="3e8f9-115">列出 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-115">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="3e8f9-116">获取 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-116">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="3e8f9-117">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-117">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="3e8f9-118">读取 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-118">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="3e8f9-119">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-119">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="3e8f9-120">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-120">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="3e8f9-121">创建新的 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-121">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="3e8f9-122">删除 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-122">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="3e8f9-123">无</span><span class="sxs-lookup"><span data-stu-id="3e8f9-123">None</span></span>|<span data-ttu-id="3e8f9-124">删除 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-124">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="3e8f9-125">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-125">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="3e8f9-126">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="3e8f9-126">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="3e8f9-127">更新 [mobileAppDependency 对象](../resources/intune-apps-mobileappdependency.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-127">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3e8f9-128">属性</span><span class="sxs-lookup"><span data-stu-id="3e8f9-128">Properties</span></span>
|<span data-ttu-id="3e8f9-129">属性</span><span class="sxs-lookup"><span data-stu-id="3e8f9-129">Property</span></span>|<span data-ttu-id="3e8f9-130">类型</span><span class="sxs-lookup"><span data-stu-id="3e8f9-130">Type</span></span>|<span data-ttu-id="3e8f9-131">说明</span><span class="sxs-lookup"><span data-stu-id="3e8f9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e8f9-132">id</span><span class="sxs-lookup"><span data-stu-id="3e8f9-132">id</span></span>|<span data-ttu-id="3e8f9-133">String</span><span class="sxs-lookup"><span data-stu-id="3e8f9-133">String</span></span>|<span data-ttu-id="3e8f9-134">关系实体 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="3e8f9-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="3e8f9-135">targetId</span><span class="sxs-lookup"><span data-stu-id="3e8f9-135">targetId</span></span>|<span data-ttu-id="3e8f9-136">String</span><span class="sxs-lookup"><span data-stu-id="3e8f9-136">String</span></span>|<span data-ttu-id="3e8f9-137">目标移动应用的应用 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="3e8f9-137">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="3e8f9-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="3e8f9-138">targetDisplayName</span></span>|<span data-ttu-id="3e8f9-139">String</span><span class="sxs-lookup"><span data-stu-id="3e8f9-139">String</span></span>|<span data-ttu-id="3e8f9-140">目标移动应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-140">The target mobile app's display name.</span></span> <span data-ttu-id="3e8f9-141">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="3e8f9-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="3e8f9-142">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="3e8f9-142">targetDisplayVersion</span></span>|<span data-ttu-id="3e8f9-143">String</span><span class="sxs-lookup"><span data-stu-id="3e8f9-143">String</span></span>|<span data-ttu-id="3e8f9-144">目标移动应用的显示版本。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-144">The target mobile app's display version.</span></span> <span data-ttu-id="3e8f9-145">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="3e8f9-145">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="3e8f9-146">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="3e8f9-146">targetPublisher</span></span>|<span data-ttu-id="3e8f9-147">String</span><span class="sxs-lookup"><span data-stu-id="3e8f9-147">String</span></span>|<span data-ttu-id="3e8f9-148">目标移动应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-148">The target mobile app's publisher.</span></span> <span data-ttu-id="3e8f9-149">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="3e8f9-149">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="3e8f9-150">targetType</span><span class="sxs-lookup"><span data-stu-id="3e8f9-150">targetType</span></span>|[<span data-ttu-id="3e8f9-151">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="3e8f9-151">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="3e8f9-152">关系类型，指示目标是父级还是子级。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-152">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="3e8f9-153">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-153">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="3e8f9-154">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-154">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="3e8f9-155">dependencyType</span><span class="sxs-lookup"><span data-stu-id="3e8f9-155">dependencyType</span></span>|[<span data-ttu-id="3e8f9-156">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="3e8f9-156">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="3e8f9-157">父应用和子应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-157">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="3e8f9-158">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-158">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="3e8f9-159">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="3e8f9-159">dependentAppCount</span></span>|<span data-ttu-id="3e8f9-160">Int32</span><span class="sxs-lookup"><span data-stu-id="3e8f9-160">Int32</span></span>|<span data-ttu-id="3e8f9-161">直接或间接依赖于父应用的应用总数。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-161">The total number of apps that directly or indirectly depend on the parent app.</span></span>|
|<span data-ttu-id="3e8f9-162">dependsOnAppCount</span><span class="sxs-lookup"><span data-stu-id="3e8f9-162">dependsOnAppCount</span></span>|<span data-ttu-id="3e8f9-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3e8f9-163">Int32</span></span>|<span data-ttu-id="3e8f9-164">子应用直接或间接依赖的应用总数。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-164">The total number of apps the child app directly or indirectly depends on.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e8f9-165">关系</span><span class="sxs-lookup"><span data-stu-id="3e8f9-165">Relationships</span></span>
<span data-ttu-id="3e8f9-166">无</span><span class="sxs-lookup"><span data-stu-id="3e8f9-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e8f9-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e8f9-167">JSON Representation</span></span>
<span data-ttu-id="3e8f9-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e8f9-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024,
  "dependsOnAppCount": 1024
}
```




