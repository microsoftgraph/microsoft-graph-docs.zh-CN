---
title: mobileAppDependency 资源类型
description: 描述两个移动应用之间的依赖关系类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b55faee86852d8b7070850a4c14a2df8fe82631
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052738"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="b0397-103">mobileAppDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0397-103">mobileAppDependency resource type</span></span>

<span data-ttu-id="b0397-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0397-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0397-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0397-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0397-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0397-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0397-107">描述两个移动应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="b0397-107">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="b0397-108">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b0397-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b0397-109">方法</span><span class="sxs-lookup"><span data-stu-id="b0397-109">Methods</span></span>
|<span data-ttu-id="b0397-110">方法</span><span class="sxs-lookup"><span data-stu-id="b0397-110">Method</span></span>|<span data-ttu-id="b0397-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="b0397-111">Return Type</span></span>|<span data-ttu-id="b0397-112">说明</span><span class="sxs-lookup"><span data-stu-id="b0397-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0397-113">列出 mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="b0397-113">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="b0397-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b0397-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="b0397-115">列出 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0397-115">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="b0397-116">获取 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-116">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="b0397-117">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-117">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="b0397-118">读取 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b0397-118">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="b0397-119">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-119">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="b0397-120">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-120">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="b0397-121">创建新的 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b0397-121">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="b0397-122">删除 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-122">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="b0397-123">无</span><span class="sxs-lookup"><span data-stu-id="b0397-123">None</span></span>|<span data-ttu-id="b0397-124">删除 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="b0397-124">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="b0397-125">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-125">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="b0397-126">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b0397-126">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="b0397-127">更新 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b0397-127">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0397-128">属性</span><span class="sxs-lookup"><span data-stu-id="b0397-128">Properties</span></span>
|<span data-ttu-id="b0397-129">属性</span><span class="sxs-lookup"><span data-stu-id="b0397-129">Property</span></span>|<span data-ttu-id="b0397-130">类型</span><span class="sxs-lookup"><span data-stu-id="b0397-130">Type</span></span>|<span data-ttu-id="b0397-131">说明</span><span class="sxs-lookup"><span data-stu-id="b0397-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0397-132">id</span><span class="sxs-lookup"><span data-stu-id="b0397-132">id</span></span>|<span data-ttu-id="b0397-133">String</span><span class="sxs-lookup"><span data-stu-id="b0397-133">String</span></span>|<span data-ttu-id="b0397-134">关系实体 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b0397-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b0397-135">targetId</span><span class="sxs-lookup"><span data-stu-id="b0397-135">targetId</span></span>|<span data-ttu-id="b0397-136">String</span><span class="sxs-lookup"><span data-stu-id="b0397-136">String</span></span>|<span data-ttu-id="b0397-137">目标移动应用程序的应用程序 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b0397-137">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b0397-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="b0397-138">targetDisplayName</span></span>|<span data-ttu-id="b0397-139">String</span><span class="sxs-lookup"><span data-stu-id="b0397-139">String</span></span>|<span data-ttu-id="b0397-140">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b0397-140">The target mobile app's display name.</span></span> <span data-ttu-id="b0397-141">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b0397-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b0397-142">targetType</span><span class="sxs-lookup"><span data-stu-id="b0397-142">targetType</span></span>|[<span data-ttu-id="b0397-143">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="b0397-143">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="b0397-144">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="b0397-144">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="b0397-145">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="b0397-145">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="b0397-146">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="b0397-146">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="b0397-147">dependencyType</span><span class="sxs-lookup"><span data-stu-id="b0397-147">dependencyType</span></span>|[<span data-ttu-id="b0397-148">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="b0397-148">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="b0397-149">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="b0397-149">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="b0397-150">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="b0397-150">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="b0397-151">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b0397-151">dependentAppCount</span></span>|<span data-ttu-id="b0397-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b0397-152">Int32</span></span>|<span data-ttu-id="b0397-153">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="b0397-153">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0397-154">关系</span><span class="sxs-lookup"><span data-stu-id="b0397-154">Relationships</span></span>
<span data-ttu-id="b0397-155">无</span><span class="sxs-lookup"><span data-stu-id="b0397-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0397-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0397-156">JSON Representation</span></span>
<span data-ttu-id="b0397-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0397-157">Here is a JSON representation of the resource.</span></span>
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
  "targetType": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```






