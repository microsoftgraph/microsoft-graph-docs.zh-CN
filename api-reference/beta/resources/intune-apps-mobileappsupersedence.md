---
title: mobileAppSupersedence 资源类型
description: 介绍两个移动应用之间的取代关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46a19d4032a661bc1f17161d2fdadde774558bcb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973966"
---
# <a name="mobileappsupersedence-resource-type"></a><span data-ttu-id="4f8b1-103">mobileAppSupersedence 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f8b1-103">mobileAppSupersedence resource type</span></span>

<span data-ttu-id="4f8b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f8b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f8b1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f8b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f8b1-107">介绍两个移动应用之间的取代关系。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-107">Describes a supersedence relationship between two mobile apps.</span></span>


<span data-ttu-id="4f8b1-108">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4f8b1-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4f8b1-109">方法</span><span class="sxs-lookup"><span data-stu-id="4f8b1-109">Methods</span></span>
|<span data-ttu-id="4f8b1-110">方法</span><span class="sxs-lookup"><span data-stu-id="4f8b1-110">Method</span></span>|<span data-ttu-id="4f8b1-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f8b1-111">Return Type</span></span>|<span data-ttu-id="4f8b1-112">说明</span><span class="sxs-lookup"><span data-stu-id="4f8b1-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f8b1-113">列出 mobileAppSupersedences</span><span class="sxs-lookup"><span data-stu-id="4f8b1-113">List mobileAppSupersedences</span></span>](../api/intune-apps-mobileappsupersedence-list.md)|<span data-ttu-id="4f8b1-114">[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4f8b1-114">[mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) collection</span></span>|<span data-ttu-id="4f8b1-115">列出 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-115">List properties and relationships of the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) objects.</span></span>|
|[<span data-ttu-id="4f8b1-116">获取 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-116">Get mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-get.md)|[<span data-ttu-id="4f8b1-117">mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-117">mobileAppSupersedence</span></span>](../resources/intune-apps-mobileappsupersedence.md)|<span data-ttu-id="4f8b1-118">读取 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-118">Read properties and relationships of the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>|
|[<span data-ttu-id="4f8b1-119">创建 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-119">Create mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-create.md)|[<span data-ttu-id="4f8b1-120">mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-120">mobileAppSupersedence</span></span>](../resources/intune-apps-mobileappsupersedence.md)|<span data-ttu-id="4f8b1-121">创建新的 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-121">Create a new [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>|
|[<span data-ttu-id="4f8b1-122">删除 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-122">Delete mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-delete.md)|<span data-ttu-id="4f8b1-123">无</span><span class="sxs-lookup"><span data-stu-id="4f8b1-123">None</span></span>|<span data-ttu-id="4f8b1-124">删除 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md)。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-124">Deletes a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span></span>|
|[<span data-ttu-id="4f8b1-125">更新 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-125">Update mobileAppSupersedence</span></span>](../api/intune-apps-mobileappsupersedence-update.md)|[<span data-ttu-id="4f8b1-126">mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="4f8b1-126">mobileAppSupersedence</span></span>](../resources/intune-apps-mobileappsupersedence.md)|<span data-ttu-id="4f8b1-127">更新 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-127">Update the properties of a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4f8b1-128">属性</span><span class="sxs-lookup"><span data-stu-id="4f8b1-128">Properties</span></span>
|<span data-ttu-id="4f8b1-129">属性</span><span class="sxs-lookup"><span data-stu-id="4f8b1-129">Property</span></span>|<span data-ttu-id="4f8b1-130">类型</span><span class="sxs-lookup"><span data-stu-id="4f8b1-130">Type</span></span>|<span data-ttu-id="4f8b1-131">说明</span><span class="sxs-lookup"><span data-stu-id="4f8b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f8b1-132">id</span><span class="sxs-lookup"><span data-stu-id="4f8b1-132">id</span></span>|<span data-ttu-id="4f8b1-133">String</span><span class="sxs-lookup"><span data-stu-id="4f8b1-133">String</span></span>|<span data-ttu-id="4f8b1-134">关系实体 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4f8b1-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4f8b1-135">targetId</span><span class="sxs-lookup"><span data-stu-id="4f8b1-135">targetId</span></span>|<span data-ttu-id="4f8b1-136">String</span><span class="sxs-lookup"><span data-stu-id="4f8b1-136">String</span></span>|<span data-ttu-id="4f8b1-137">目标移动应用程序的应用程序 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4f8b1-137">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4f8b1-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="4f8b1-138">targetDisplayName</span></span>|<span data-ttu-id="4f8b1-139">String</span><span class="sxs-lookup"><span data-stu-id="4f8b1-139">String</span></span>|<span data-ttu-id="4f8b1-140">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-140">The target mobile app's display name.</span></span> <span data-ttu-id="4f8b1-141">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4f8b1-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4f8b1-142">targetType</span><span class="sxs-lookup"><span data-stu-id="4f8b1-142">targetType</span></span>|[<span data-ttu-id="4f8b1-143">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="4f8b1-143">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="4f8b1-144">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-144">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="4f8b1-145">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-145">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="4f8b1-146">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-146">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="4f8b1-147">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="4f8b1-147">supersedenceType</span></span>|[<span data-ttu-id="4f8b1-148">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="4f8b1-148">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="4f8b1-149">父应用和子应用之间的取代关系类型。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-149">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="4f8b1-150">可取值为：`update`、`replace`。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-150">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="4f8b1-151">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="4f8b1-151">supersededAppCount</span></span>|<span data-ttu-id="4f8b1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4f8b1-152">Int32</span></span>|<span data-ttu-id="4f8b1-153">由子应用直接或间接取代的应用程序总数。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-153">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="4f8b1-154">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="4f8b1-154">supersedingAppCount</span></span>|<span data-ttu-id="4f8b1-155">Int32</span><span class="sxs-lookup"><span data-stu-id="4f8b1-155">Int32</span></span>|<span data-ttu-id="4f8b1-156">直接或间接取代父应用程序的应用程序总数量。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-156">The total number of apps directly or indirectly superseding the parent app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f8b1-157">关系</span><span class="sxs-lookup"><span data-stu-id="4f8b1-157">Relationships</span></span>
<span data-ttu-id="4f8b1-158">无</span><span class="sxs-lookup"><span data-stu-id="4f8b1-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f8b1-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f8b1-159">JSON Representation</span></span>
<span data-ttu-id="4f8b1-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f8b1-160">Here is a JSON representation of the resource.</span></span>
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
  "targetType": "String",
  "supersedenceType": "String",
  "supersededAppCount": 1024,
  "supersedingAppCount": 1024
}
```






