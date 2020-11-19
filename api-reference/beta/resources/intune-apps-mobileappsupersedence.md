---
title: mobileAppSupersedence 资源类型
description: 介绍两个移动应用之间的取代关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1e63bdfce275b83587557304f79a8490eb45a68c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217128"
---
# <a name="mobileappsupersedence-resource-type"></a><span data-ttu-id="df5ea-103">mobileAppSupersedence 资源类型</span><span class="sxs-lookup"><span data-stu-id="df5ea-103">mobileAppSupersedence resource type</span></span>

<span data-ttu-id="df5ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df5ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df5ea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df5ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df5ea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df5ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df5ea-107">介绍两个移动应用之间的取代关系。</span><span class="sxs-lookup"><span data-stu-id="df5ea-107">Describes a supersedence relationship between two mobile apps.</span></span>


<span data-ttu-id="df5ea-108">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="df5ea-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="df5ea-109">方法</span><span class="sxs-lookup"><span data-stu-id="df5ea-109">Methods</span></span>
|<span data-ttu-id="df5ea-110">方法</span><span class="sxs-lookup"><span data-stu-id="df5ea-110">Method</span></span>|<span data-ttu-id="df5ea-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="df5ea-111">Return Type</span></span>|<span data-ttu-id="df5ea-112">说明</span><span class="sxs-lookup"><span data-stu-id="df5ea-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df5ea-113">列出 mobileAppSupersedences</span><span class="sxs-lookup"><span data-stu-id="df5ea-113">List mobileAppSupersedences</span></span>](../api/intune-apps-mobileappsupersedence-list.md)|<span data-ttu-id="df5ea-114">[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df5ea-114">[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) collection</span></span>|<span data-ttu-id="df5ea-115">列出 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df5ea-115">List properties and relationships of the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) objects.</span></span>|
|[<span data-ttu-id="df5ea-116">获取 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-116">Get mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-get.md)|[<span data-ttu-id="df5ea-117">mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-117">mobileAppSupersedence</span></span>](../resources/intune-apps-mobileappsupersedence.md)|<span data-ttu-id="df5ea-118">读取 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="df5ea-118">Read properties and relationships of the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>|
|[<span data-ttu-id="df5ea-119">创建 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-119">Create mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-create.md)|[<span data-ttu-id="df5ea-120">mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-120">mobileAppSupersedence</span></span>](../resources/intune-apps-mobileappsupersedence.md)|<span data-ttu-id="df5ea-121">创建新的 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df5ea-121">Create a new [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>|
|[<span data-ttu-id="df5ea-122">删除 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-122">Delete mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-delete.md)|<span data-ttu-id="df5ea-123">无</span><span class="sxs-lookup"><span data-stu-id="df5ea-123">None</span></span>|<span data-ttu-id="df5ea-124">删除 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)。</span><span class="sxs-lookup"><span data-stu-id="df5ea-124">Deletes a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span></span>|
|[<span data-ttu-id="df5ea-125">更新 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-125">Update mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-update.md)|[<span data-ttu-id="df5ea-126">mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="df5ea-126">mobileAppSupersedence</span></span>](../resources/intune-apps-mobileappsupersedence.md)|<span data-ttu-id="df5ea-127">更新 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df5ea-127">Update the properties of a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="df5ea-128">属性</span><span class="sxs-lookup"><span data-stu-id="df5ea-128">Properties</span></span>
|<span data-ttu-id="df5ea-129">属性</span><span class="sxs-lookup"><span data-stu-id="df5ea-129">Property</span></span>|<span data-ttu-id="df5ea-130">类型</span><span class="sxs-lookup"><span data-stu-id="df5ea-130">Type</span></span>|<span data-ttu-id="df5ea-131">说明</span><span class="sxs-lookup"><span data-stu-id="df5ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df5ea-132">id</span><span class="sxs-lookup"><span data-stu-id="df5ea-132">id</span></span>|<span data-ttu-id="df5ea-133">String</span><span class="sxs-lookup"><span data-stu-id="df5ea-133">String</span></span>|<span data-ttu-id="df5ea-134">关系实体 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="df5ea-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="df5ea-135">targetId</span><span class="sxs-lookup"><span data-stu-id="df5ea-135">targetId</span></span>|<span data-ttu-id="df5ea-136">String</span><span class="sxs-lookup"><span data-stu-id="df5ea-136">String</span></span>|<span data-ttu-id="df5ea-137">目标移动应用程序的应用程序 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="df5ea-137">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="df5ea-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="df5ea-138">targetDisplayName</span></span>|<span data-ttu-id="df5ea-139">String</span><span class="sxs-lookup"><span data-stu-id="df5ea-139">String</span></span>|<span data-ttu-id="df5ea-140">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="df5ea-140">The target mobile app's display name.</span></span> <span data-ttu-id="df5ea-141">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="df5ea-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="df5ea-142">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="df5ea-142">targetDisplayVersion</span></span>|<span data-ttu-id="df5ea-143">String</span><span class="sxs-lookup"><span data-stu-id="df5ea-143">String</span></span>|<span data-ttu-id="df5ea-144">目标移动应用程序的显示版本。</span><span class="sxs-lookup"><span data-stu-id="df5ea-144">The target mobile app's display version.</span></span> <span data-ttu-id="df5ea-145">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="df5ea-145">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="df5ea-146">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="df5ea-146">targetPublisher</span></span>|<span data-ttu-id="df5ea-147">String</span><span class="sxs-lookup"><span data-stu-id="df5ea-147">String</span></span>|<span data-ttu-id="df5ea-148">目标移动应用程序的发布者。</span><span class="sxs-lookup"><span data-stu-id="df5ea-148">The target mobile app's publisher.</span></span> <span data-ttu-id="df5ea-149">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="df5ea-149">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="df5ea-150">targetType</span><span class="sxs-lookup"><span data-stu-id="df5ea-150">targetType</span></span>|[<span data-ttu-id="df5ea-151">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="df5ea-151">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="df5ea-152">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="df5ea-152">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="df5ea-153">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="df5ea-153">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="df5ea-154">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="df5ea-154">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="df5ea-155">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="df5ea-155">supersedenceType</span></span>|[<span data-ttu-id="df5ea-156">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="df5ea-156">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="df5ea-157">父应用和子应用之间的取代关系类型。</span><span class="sxs-lookup"><span data-stu-id="df5ea-157">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="df5ea-158">可取值为：`update`、`replace`。</span><span class="sxs-lookup"><span data-stu-id="df5ea-158">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="df5ea-159">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="df5ea-159">supersededAppCount</span></span>|<span data-ttu-id="df5ea-160">Int32</span><span class="sxs-lookup"><span data-stu-id="df5ea-160">Int32</span></span>|<span data-ttu-id="df5ea-161">由子应用直接或间接取代的应用程序总数。</span><span class="sxs-lookup"><span data-stu-id="df5ea-161">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="df5ea-162">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="df5ea-162">supersedingAppCount</span></span>|<span data-ttu-id="df5ea-163">Int32</span><span class="sxs-lookup"><span data-stu-id="df5ea-163">Int32</span></span>|<span data-ttu-id="df5ea-164">直接或间接取代父应用程序的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="df5ea-164">The total number of apps directly or indirectly superseding the parent app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df5ea-165">关系</span><span class="sxs-lookup"><span data-stu-id="df5ea-165">Relationships</span></span>
<span data-ttu-id="df5ea-166">无</span><span class="sxs-lookup"><span data-stu-id="df5ea-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df5ea-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df5ea-167">JSON Representation</span></span>
<span data-ttu-id="df5ea-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df5ea-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppSupersedence"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "targetDisplayVersion": "String",
  "targetPublisher": "String",
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```




