---
title: mobileAppDependency 资源类型
description: 描述两个移动应用之间的依赖关系类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 99d5458d52e22bf4fd88f16eaef1deed6c2b7873
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342129"
---
# <a name="mobileappdependency-resource-type"></a><span data-ttu-id="c7506-103">mobileAppDependency 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7506-103">mobileAppDependency resource type</span></span>

> <span data-ttu-id="c7506-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7506-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7506-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7506-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7506-106">描述两个移动应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="c7506-106">Describes a dependency type between two mobile apps.</span></span>


<span data-ttu-id="c7506-107">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c7506-107">Inherits from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c7506-108">方法</span><span class="sxs-lookup"><span data-stu-id="c7506-108">Methods</span></span>
|<span data-ttu-id="c7506-109">方法</span><span class="sxs-lookup"><span data-stu-id="c7506-109">Method</span></span>|<span data-ttu-id="c7506-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c7506-110">Return Type</span></span>|<span data-ttu-id="c7506-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7506-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c7506-112">列出 mobileAppDependencies</span><span class="sxs-lookup"><span data-stu-id="c7506-112">List mobileAppDependencies</span></span>](../api/intune-apps-mobileappdependency-list.md)|<span data-ttu-id="c7506-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)集合</span><span class="sxs-lookup"><span data-stu-id="c7506-113">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md) collection</span></span>|<span data-ttu-id="c7506-114">列出[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7506-114">List properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) objects.</span></span>|
|[<span data-ttu-id="c7506-115">获取 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-115">Get mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-get.md)|[<span data-ttu-id="c7506-116">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-116">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="c7506-117">读取[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7506-117">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="c7506-118">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-118">Create mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-create.md)|[<span data-ttu-id="c7506-119">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-119">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="c7506-120">创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7506-120">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|
|[<span data-ttu-id="c7506-121">删除 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-121">Delete mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-delete.md)|<span data-ttu-id="c7506-122">无</span><span class="sxs-lookup"><span data-stu-id="c7506-122">None</span></span>|<span data-ttu-id="c7506-123">删除[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="c7506-123">Deletes a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>|
|[<span data-ttu-id="c7506-124">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-124">Update mobileAppDependency</span></span>](../api/intune-apps-mobileappdependency-update.md)|[<span data-ttu-id="c7506-125">mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c7506-125">mobileAppDependency</span></span>](../resources/intune-apps-mobileappdependency.md)|<span data-ttu-id="c7506-126">更新[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c7506-126">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c7506-127">属性</span><span class="sxs-lookup"><span data-stu-id="c7506-127">Properties</span></span>
|<span data-ttu-id="c7506-128">属性</span><span class="sxs-lookup"><span data-stu-id="c7506-128">Property</span></span>|<span data-ttu-id="c7506-129">类型</span><span class="sxs-lookup"><span data-stu-id="c7506-129">Type</span></span>|<span data-ttu-id="c7506-130">说明</span><span class="sxs-lookup"><span data-stu-id="c7506-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7506-131">id</span><span class="sxs-lookup"><span data-stu-id="c7506-131">id</span></span>|<span data-ttu-id="c7506-132">String</span><span class="sxs-lookup"><span data-stu-id="c7506-132">String</span></span>|<span data-ttu-id="c7506-133">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c7506-133">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c7506-134">targetId</span><span class="sxs-lookup"><span data-stu-id="c7506-134">targetId</span></span>|<span data-ttu-id="c7506-135">String</span><span class="sxs-lookup"><span data-stu-id="c7506-135">String</span></span>|<span data-ttu-id="c7506-136">目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c7506-136">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c7506-137">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="c7506-137">targetDisplayName</span></span>|<span data-ttu-id="c7506-138">String</span><span class="sxs-lookup"><span data-stu-id="c7506-138">String</span></span>|<span data-ttu-id="c7506-139">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c7506-139">The target child mobile app's display name.</span></span> <span data-ttu-id="c7506-140">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c7506-140">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c7506-141">dependencyType</span><span class="sxs-lookup"><span data-stu-id="c7506-141">dependencyType</span></span>|[<span data-ttu-id="c7506-142">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="c7506-142">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="c7506-143">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="c7506-143">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="c7506-144">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="c7506-144">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="c7506-145">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c7506-145">dependentAppCount</span></span>|<span data-ttu-id="c7506-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c7506-146">Int32</span></span>|<span data-ttu-id="c7506-147">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="c7506-147">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7506-148">关系</span><span class="sxs-lookup"><span data-stu-id="c7506-148">Relationships</span></span>
<span data-ttu-id="c7506-149">无</span><span class="sxs-lookup"><span data-stu-id="c7506-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7506-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7506-150">JSON Representation</span></span>
<span data-ttu-id="c7506-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7506-151">Here is a JSON representation of the resource.</span></span>
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



