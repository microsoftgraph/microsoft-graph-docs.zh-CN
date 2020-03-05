---
title: windowsFeatureUpdateProfile 资源类型
description: Windows 功能更新配置文件
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3471b5e20c16804721cdeccbd3b1a38bbde13a67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523434"
---
# <a name="windowsfeatureupdateprofile-resource-type"></a><span data-ttu-id="4eb6a-103">windowsFeatureUpdateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="4eb6a-103">windowsFeatureUpdateProfile resource type</span></span>

<span data-ttu-id="4eb6a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4eb6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4eb6a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4eb6a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eb6a-107">Windows 功能更新配置文件</span><span class="sxs-lookup"><span data-stu-id="4eb6a-107">Windows Feature Update Profile</span></span>

## <a name="methods"></a><span data-ttu-id="4eb6a-108">方法</span><span class="sxs-lookup"><span data-stu-id="4eb6a-108">Methods</span></span>
|<span data-ttu-id="4eb6a-109">方法</span><span class="sxs-lookup"><span data-stu-id="4eb6a-109">Method</span></span>|<span data-ttu-id="4eb6a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4eb6a-110">Return Type</span></span>|<span data-ttu-id="4eb6a-111">说明</span><span class="sxs-lookup"><span data-stu-id="4eb6a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4eb6a-112">列出 windowsFeatureUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="4eb6a-112">List windowsFeatureUpdateProfiles</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-list.md)|<span data-ttu-id="4eb6a-113">[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="4eb6a-113">[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) collection</span></span>|<span data-ttu-id="4eb6a-114">列出[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-114">List properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects.</span></span>|
|[<span data-ttu-id="4eb6a-115">获取 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-115">Get windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-get.md)|[<span data-ttu-id="4eb6a-116">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-116">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="4eb6a-117">读取[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-117">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="4eb6a-118">创建 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-118">Create windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-create.md)|[<span data-ttu-id="4eb6a-119">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-119">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="4eb6a-120">创建新的[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-120">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="4eb6a-121">删除 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-121">Delete windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|<span data-ttu-id="4eb6a-122">无</span><span class="sxs-lookup"><span data-stu-id="4eb6a-122">None</span></span>|<span data-ttu-id="4eb6a-123">删除[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-123">Deletes a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>|
|[<span data-ttu-id="4eb6a-124">更新 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-124">Update windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[<span data-ttu-id="4eb6a-125">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="4eb6a-125">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="4eb6a-126">更新[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-126">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="4eb6a-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="4eb6a-127">assign action</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|<span data-ttu-id="4eb6a-128">无</span><span class="sxs-lookup"><span data-stu-id="4eb6a-128">None</span></span>|<span data-ttu-id="4eb6a-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4eb6a-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4eb6a-130">属性</span><span class="sxs-lookup"><span data-stu-id="4eb6a-130">Properties</span></span>
|<span data-ttu-id="4eb6a-131">属性</span><span class="sxs-lookup"><span data-stu-id="4eb6a-131">Property</span></span>|<span data-ttu-id="4eb6a-132">类型</span><span class="sxs-lookup"><span data-stu-id="4eb6a-132">Type</span></span>|<span data-ttu-id="4eb6a-133">说明</span><span class="sxs-lookup"><span data-stu-id="4eb6a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb6a-134">id</span><span class="sxs-lookup"><span data-stu-id="4eb6a-134">id</span></span>|<span data-ttu-id="4eb6a-135">字符串</span><span class="sxs-lookup"><span data-stu-id="4eb6a-135">String</span></span>|<span data-ttu-id="4eb6a-136">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-136">The Identifier of the entity.</span></span>|
|<span data-ttu-id="4eb6a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4eb6a-137">displayName</span></span>|<span data-ttu-id="4eb6a-138">String</span><span class="sxs-lookup"><span data-stu-id="4eb6a-138">String</span></span>|<span data-ttu-id="4eb6a-139">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-139">The display name of the profile.</span></span>|
|<span data-ttu-id="4eb6a-140">说明</span><span class="sxs-lookup"><span data-stu-id="4eb6a-140">description</span></span>|<span data-ttu-id="4eb6a-141">String</span><span class="sxs-lookup"><span data-stu-id="4eb6a-141">String</span></span>|<span data-ttu-id="4eb6a-142">用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-142">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="4eb6a-143">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="4eb6a-143">featureUpdateVersion</span></span>|<span data-ttu-id="4eb6a-144">String</span><span class="sxs-lookup"><span data-stu-id="4eb6a-144">String</span></span>|<span data-ttu-id="4eb6a-145">将部署到此配置文件目标的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-145">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="4eb6a-146">版本可以是任何受支持的版本，例如，1709、1803或1809等。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-146">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="4eb6a-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb6a-147">createdDateTime</span></span>|<span data-ttu-id="4eb6a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb6a-148">DateTimeOffset</span></span>|<span data-ttu-id="4eb6a-149">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-149">The date time that the profile was created.</span></span>|
|<span data-ttu-id="4eb6a-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eb6a-150">lastModifiedDateTime</span></span>|<span data-ttu-id="4eb6a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eb6a-151">DateTimeOffset</span></span>|<span data-ttu-id="4eb6a-152">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-152">The date time that the profile was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eb6a-153">关系</span><span class="sxs-lookup"><span data-stu-id="4eb6a-153">Relationships</span></span>
|<span data-ttu-id="4eb6a-154">关系</span><span class="sxs-lookup"><span data-stu-id="4eb6a-154">Relationship</span></span>|<span data-ttu-id="4eb6a-155">类型</span><span class="sxs-lookup"><span data-stu-id="4eb6a-155">Type</span></span>|<span data-ttu-id="4eb6a-156">说明</span><span class="sxs-lookup"><span data-stu-id="4eb6a-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb6a-157">assignments</span><span class="sxs-lookup"><span data-stu-id="4eb6a-157">assignments</span></span>|<span data-ttu-id="4eb6a-158">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="4eb6a-158">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="4eb6a-159">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-159">The list of group assignments of the profile.</span></span>|
|<span data-ttu-id="4eb6a-160">deviceUpdateStates</span><span class="sxs-lookup"><span data-stu-id="4eb6a-160">deviceUpdateStates</span></span>|<span data-ttu-id="4eb6a-161">[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="4eb6a-161">[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) collection</span></span>|<span data-ttu-id="4eb6a-162">此配置文件指向的设备状态的列表</span><span class="sxs-lookup"><span data-stu-id="4eb6a-162">The list of device states this profile targeted to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4eb6a-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4eb6a-163">JSON Representation</span></span>
<span data-ttu-id="4eb6a-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eb6a-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "featureUpdateVersion": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



