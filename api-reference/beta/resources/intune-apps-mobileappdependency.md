---
title: mobileAppDependency 资源类型
description: 描述两个移动应用之间的依赖关系类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 42f87c57f7df7c60e75070ed9ac0a579cb436f91
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440390"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="88055-103">mobileAppDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="88055-103">mobileAppDependency resource type</span></span>

<span data-ttu-id="88055-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88055-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88055-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88055-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88055-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88055-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88055-107">描述两个移动应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="88055-107">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="88055-108">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="88055-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="88055-109">方法</span><span class="sxs-lookup"><span data-stu-id="88055-109">Methods</span></span>
|<span data-ttu-id="88055-110">方法</span><span class="sxs-lookup"><span data-stu-id="88055-110">Method</span></span>|<span data-ttu-id="88055-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="88055-111">Return Type</span></span>|<span data-ttu-id="88055-112">说明</span><span class="sxs-lookup"><span data-stu-id="88055-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="88055-113">列出 mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="88055-113">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="88055-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="88055-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="88055-115">列出[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88055-115">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="88055-116">获取 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-116">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="88055-117">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-117">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="88055-118">读取[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="88055-118">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="88055-119">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-119">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="88055-120">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-120">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="88055-121">创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88055-121">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="88055-122">删除 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-122">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="88055-123">无</span><span class="sxs-lookup"><span data-stu-id="88055-123">None</span></span>|<span data-ttu-id="88055-124">删除[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="88055-124">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="88055-125">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-125">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="88055-126">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="88055-126">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="88055-127">更新[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88055-127">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="88055-128">属性</span><span class="sxs-lookup"><span data-stu-id="88055-128">Properties</span></span>
|<span data-ttu-id="88055-129">属性</span><span class="sxs-lookup"><span data-stu-id="88055-129">Property</span></span>|<span data-ttu-id="88055-130">类型</span><span class="sxs-lookup"><span data-stu-id="88055-130">Type</span></span>|<span data-ttu-id="88055-131">说明</span><span class="sxs-lookup"><span data-stu-id="88055-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88055-132">id</span><span class="sxs-lookup"><span data-stu-id="88055-132">id</span></span>|<span data-ttu-id="88055-133">String</span><span class="sxs-lookup"><span data-stu-id="88055-133">String</span></span>|<span data-ttu-id="88055-134">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="88055-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="88055-135">targetId</span><span class="sxs-lookup"><span data-stu-id="88055-135">targetId</span></span>|<span data-ttu-id="88055-136">String</span><span class="sxs-lookup"><span data-stu-id="88055-136">String</span></span>|<span data-ttu-id="88055-137">目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="88055-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="88055-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="88055-138">targetDisplayName</span></span>|<span data-ttu-id="88055-139">String</span><span class="sxs-lookup"><span data-stu-id="88055-139">String</span></span>|<span data-ttu-id="88055-140">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="88055-140">The target child mobile app's display name.</span></span> <span data-ttu-id="88055-141">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="88055-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="88055-142">dependencyType</span><span class="sxs-lookup"><span data-stu-id="88055-142">dependencyType</span></span>|[<span data-ttu-id="88055-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="88055-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="88055-144">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="88055-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="88055-145">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="88055-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="88055-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="88055-146">dependentAppCount</span></span>|<span data-ttu-id="88055-147">Int32</span><span class="sxs-lookup"><span data-stu-id="88055-147">Int32</span></span>|<span data-ttu-id="88055-148">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="88055-148">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88055-149">关系</span><span class="sxs-lookup"><span data-stu-id="88055-149">Relationships</span></span>
<span data-ttu-id="88055-150">无</span><span class="sxs-lookup"><span data-stu-id="88055-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88055-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88055-151">JSON Representation</span></span>
<span data-ttu-id="88055-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88055-152">Here is a JSON representation of the resource.</span></span>
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
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```



