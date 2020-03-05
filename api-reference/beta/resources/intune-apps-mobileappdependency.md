---
title: mobileAppDependency 资源类型
description: 描述两个移动应用之间的依赖关系类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8140b430f8652b552c3dd2cdb85f22ba4a6190b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491758"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="d7a5a-103">mobileAppDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7a5a-103">mobileAppDependency resource type</span></span>

<span data-ttu-id="d7a5a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d7a5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7a5a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7a5a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7a5a-107">描述两个移动应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-107">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="d7a5a-108">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d7a5a-108">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d7a5a-109">方法</span><span class="sxs-lookup"><span data-stu-id="d7a5a-109">Methods</span></span>
|<span data-ttu-id="d7a5a-110">方法</span><span class="sxs-lookup"><span data-stu-id="d7a5a-110">Method</span></span>|<span data-ttu-id="d7a5a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7a5a-111">Return Type</span></span>|<span data-ttu-id="d7a5a-112">说明</span><span class="sxs-lookup"><span data-stu-id="d7a5a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d7a5a-113">列出 mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="d7a5a-113">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="d7a5a-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="d7a5a-114">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="d7a5a-115">列出[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-115">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="d7a5a-116">获取 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-116">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="d7a5a-117">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-117">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="d7a5a-118">读取[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-118">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="d7a5a-119">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-119">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="d7a5a-120">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-120">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="d7a5a-121">创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-121">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="d7a5a-122">删除 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-122">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="d7a5a-123">无</span><span class="sxs-lookup"><span data-stu-id="d7a5a-123">None</span></span>|<span data-ttu-id="d7a5a-124">删除[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-124">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="d7a5a-125">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-125">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="d7a5a-126">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d7a5a-126">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="d7a5a-127">更新[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-127">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7a5a-128">属性</span><span class="sxs-lookup"><span data-stu-id="d7a5a-128">Properties</span></span>
|<span data-ttu-id="d7a5a-129">属性</span><span class="sxs-lookup"><span data-stu-id="d7a5a-129">Property</span></span>|<span data-ttu-id="d7a5a-130">类型</span><span class="sxs-lookup"><span data-stu-id="d7a5a-130">Type</span></span>|<span data-ttu-id="d7a5a-131">说明</span><span class="sxs-lookup"><span data-stu-id="d7a5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7a5a-132">id</span><span class="sxs-lookup"><span data-stu-id="d7a5a-132">id</span></span>|<span data-ttu-id="d7a5a-133">String</span><span class="sxs-lookup"><span data-stu-id="d7a5a-133">String</span></span>|<span data-ttu-id="d7a5a-134">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d7a5a-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d7a5a-135">targetId</span><span class="sxs-lookup"><span data-stu-id="d7a5a-135">targetId</span></span>|<span data-ttu-id="d7a5a-136">String</span><span class="sxs-lookup"><span data-stu-id="d7a5a-136">String</span></span>|<span data-ttu-id="d7a5a-137">目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d7a5a-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d7a5a-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7a5a-138">targetDisplayName</span></span>|<span data-ttu-id="d7a5a-139">String</span><span class="sxs-lookup"><span data-stu-id="d7a5a-139">String</span></span>|<span data-ttu-id="d7a5a-140">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-140">The target child mobile app's display name.</span></span> <span data-ttu-id="d7a5a-141">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d7a5a-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d7a5a-142">dependencyType</span><span class="sxs-lookup"><span data-stu-id="d7a5a-142">dependencyType</span></span>|[<span data-ttu-id="d7a5a-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="d7a5a-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="d7a5a-144">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="d7a5a-145">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="d7a5a-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d7a5a-146">dependentAppCount</span></span>|<span data-ttu-id="d7a5a-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d7a5a-147">Int32</span></span>|<span data-ttu-id="d7a5a-148">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-148">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7a5a-149">关系</span><span class="sxs-lookup"><span data-stu-id="d7a5a-149">Relationships</span></span>
<span data-ttu-id="d7a5a-150">无</span><span class="sxs-lookup"><span data-stu-id="d7a5a-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7a5a-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7a5a-151">JSON Representation</span></span>
<span data-ttu-id="d7a5a-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7a5a-152">Here is a JSON representation of the resource.</span></span>
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



