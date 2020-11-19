---
title: mobileAppDependency 资源类型
description: 描述两个移动应用之间的依赖关系类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 525e094350a3ce255d0a695ad2631485087e3d37
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280956"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="d9e36-103">mobileAppDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9e36-103">mobileAppDependency resource type</span></span>

<span data-ttu-id="d9e36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9e36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9e36-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d9e36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9e36-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d9e36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9e36-107">描述两个移动应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="d9e36-107">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="d9e36-108">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d9e36-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d9e36-109">Methods</span><span class="sxs-lookup"><span data-stu-id="d9e36-109">Methods</span></span>
|<span data-ttu-id="d9e36-110">方法</span><span class="sxs-lookup"><span data-stu-id="d9e36-110">Method</span></span>|<span data-ttu-id="d9e36-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d9e36-111">Return Type</span></span>|<span data-ttu-id="d9e36-112">Description</span><span class="sxs-lookup"><span data-stu-id="d9e36-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d9e36-113">列出 mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="d9e36-113">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="d9e36-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d9e36-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="d9e36-115">列出 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9e36-115">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="d9e36-116">获取 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-116">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="d9e36-117">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-117">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="d9e36-118">读取 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d9e36-118">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="d9e36-119">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-119">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="d9e36-120">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-120">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="d9e36-121">创建新的 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e36-121">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="d9e36-122">删除 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-122">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="d9e36-123">无</span><span class="sxs-lookup"><span data-stu-id="d9e36-123">None</span></span>|<span data-ttu-id="d9e36-124">删除 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="d9e36-124">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="d9e36-125">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-125">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="d9e36-126">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d9e36-126">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="d9e36-127">更新 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e36-127">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9e36-128">属性</span><span class="sxs-lookup"><span data-stu-id="d9e36-128">Properties</span></span>
|<span data-ttu-id="d9e36-129">属性</span><span class="sxs-lookup"><span data-stu-id="d9e36-129">Property</span></span>|<span data-ttu-id="d9e36-130">类型</span><span class="sxs-lookup"><span data-stu-id="d9e36-130">Type</span></span>|<span data-ttu-id="d9e36-131">说明</span><span class="sxs-lookup"><span data-stu-id="d9e36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e36-132">id</span><span class="sxs-lookup"><span data-stu-id="d9e36-132">id</span></span>|<span data-ttu-id="d9e36-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e36-133">String</span></span>|<span data-ttu-id="d9e36-134">关系实体 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d9e36-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d9e36-135">targetId</span><span class="sxs-lookup"><span data-stu-id="d9e36-135">targetId</span></span>|<span data-ttu-id="d9e36-136">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e36-136">String</span></span>|<span data-ttu-id="d9e36-137">目标移动应用程序的应用程序 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d9e36-137">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d9e36-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="d9e36-138">targetDisplayName</span></span>|<span data-ttu-id="d9e36-139">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e36-139">String</span></span>|<span data-ttu-id="d9e36-140">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9e36-140">The target mobile app's display name.</span></span> <span data-ttu-id="d9e36-141">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d9e36-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d9e36-142">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="d9e36-142">targetDisplayVersion</span></span>|<span data-ttu-id="d9e36-143">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e36-143">String</span></span>|<span data-ttu-id="d9e36-144">目标移动应用程序的显示版本。</span><span class="sxs-lookup"><span data-stu-id="d9e36-144">The target mobile app's display version.</span></span> <span data-ttu-id="d9e36-145">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d9e36-145">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d9e36-146">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="d9e36-146">targetPublisher</span></span>|<span data-ttu-id="d9e36-147">字符串</span><span class="sxs-lookup"><span data-stu-id="d9e36-147">String</span></span>|<span data-ttu-id="d9e36-148">目标移动应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="d9e36-148">The target mobile app's publisher.</span></span> <span data-ttu-id="d9e36-149">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d9e36-149">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d9e36-150">targetType</span><span class="sxs-lookup"><span data-stu-id="d9e36-150">targetType</span></span>|[<span data-ttu-id="d9e36-151">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="d9e36-151">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="d9e36-152">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="d9e36-152">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="d9e36-153">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="d9e36-153">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="d9e36-154">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="d9e36-154">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="d9e36-155">dependencyType</span><span class="sxs-lookup"><span data-stu-id="d9e36-155">dependencyType</span></span>|[<span data-ttu-id="d9e36-156">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="d9e36-156">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="d9e36-157">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="d9e36-157">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="d9e36-158">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="d9e36-158">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="d9e36-159">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d9e36-159">dependentAppCount</span></span>|<span data-ttu-id="d9e36-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d9e36-160">Int32</span></span>|<span data-ttu-id="d9e36-161">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="d9e36-161">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9e36-162">关系</span><span class="sxs-lookup"><span data-stu-id="d9e36-162">Relationships</span></span>
<span data-ttu-id="d9e36-163">无</span><span class="sxs-lookup"><span data-stu-id="d9e36-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9e36-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9e36-164">JSON Representation</span></span>
<span data-ttu-id="d9e36-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9e36-165">Here is a JSON representation of the resource.</span></span>
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
  "dependentAppCount": 1024
}
```




