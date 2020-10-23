---
title: windowsFeatureUpdateProfile 资源类型
description: Windows 功能更新配置文件
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2157fccff9cbd6a1618b5989b91bb95edae576c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702234"
---
# <a name="windowsfeatureupdateprofile-resource-type"></a><span data-ttu-id="d3aea-103">windowsFeatureUpdateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3aea-103">windowsFeatureUpdateProfile resource type</span></span>

<span data-ttu-id="d3aea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3aea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3aea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3aea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3aea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3aea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3aea-107">Windows 功能更新配置文件</span><span class="sxs-lookup"><span data-stu-id="d3aea-107">Windows Feature Update Profile</span></span>

## <a name="methods"></a><span data-ttu-id="d3aea-108">Methods</span><span class="sxs-lookup"><span data-stu-id="d3aea-108">Methods</span></span>
|<span data-ttu-id="d3aea-109">方法</span><span class="sxs-lookup"><span data-stu-id="d3aea-109">Method</span></span>|<span data-ttu-id="d3aea-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d3aea-110">Return Type</span></span>|<span data-ttu-id="d3aea-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3aea-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3aea-112">列出 windowsFeatureUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="d3aea-112">List windowsFeatureUpdateProfiles</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-list.md)|<span data-ttu-id="d3aea-113">[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3aea-113">[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) collection</span></span>|<span data-ttu-id="d3aea-114">列出 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3aea-114">List properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects.</span></span>|
|[<span data-ttu-id="d3aea-115">获取 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-115">Get windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-get.md)|[<span data-ttu-id="d3aea-116">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-116">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="d3aea-117">读取 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d3aea-117">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="d3aea-118">创建 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-118">Create windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-create.md)|[<span data-ttu-id="d3aea-119">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-119">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="d3aea-120">创建新的 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3aea-120">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="d3aea-121">删除 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-121">Delete windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|<span data-ttu-id="d3aea-122">无</span><span class="sxs-lookup"><span data-stu-id="d3aea-122">None</span></span>|<span data-ttu-id="d3aea-123">删除 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="d3aea-123">Deletes a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>|
|[<span data-ttu-id="d3aea-124">更新 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-124">Update windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[<span data-ttu-id="d3aea-125">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d3aea-125">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="d3aea-126">更新 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d3aea-126">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="d3aea-127">分配操作</span><span class="sxs-lookup"><span data-stu-id="d3aea-127">assign action</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|<span data-ttu-id="d3aea-128">无</span><span class="sxs-lookup"><span data-stu-id="d3aea-128">None</span></span>|<span data-ttu-id="d3aea-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="d3aea-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d3aea-130">属性</span><span class="sxs-lookup"><span data-stu-id="d3aea-130">Properties</span></span>
|<span data-ttu-id="d3aea-131">属性</span><span class="sxs-lookup"><span data-stu-id="d3aea-131">Property</span></span>|<span data-ttu-id="d3aea-132">类型</span><span class="sxs-lookup"><span data-stu-id="d3aea-132">Type</span></span>|<span data-ttu-id="d3aea-133">说明</span><span class="sxs-lookup"><span data-stu-id="d3aea-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3aea-134">id</span><span class="sxs-lookup"><span data-stu-id="d3aea-134">id</span></span>|<span data-ttu-id="d3aea-135">String</span><span class="sxs-lookup"><span data-stu-id="d3aea-135">String</span></span>|<span data-ttu-id="d3aea-136">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="d3aea-136">The Identifier of the entity.</span></span>|
|<span data-ttu-id="d3aea-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d3aea-137">displayName</span></span>|<span data-ttu-id="d3aea-138">String</span><span class="sxs-lookup"><span data-stu-id="d3aea-138">String</span></span>|<span data-ttu-id="d3aea-139">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3aea-139">The display name of the profile.</span></span>|
|<span data-ttu-id="d3aea-140">说明</span><span class="sxs-lookup"><span data-stu-id="d3aea-140">description</span></span>|<span data-ttu-id="d3aea-141">String</span><span class="sxs-lookup"><span data-stu-id="d3aea-141">String</span></span>|<span data-ttu-id="d3aea-142">用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="d3aea-142">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="d3aea-143">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="d3aea-143">featureUpdateVersion</span></span>|<span data-ttu-id="d3aea-144">String</span><span class="sxs-lookup"><span data-stu-id="d3aea-144">String</span></span>|<span data-ttu-id="d3aea-145">将部署到此配置文件目标的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="d3aea-145">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="d3aea-146">版本可以是任何受支持的版本，例如，1709、1803或1809等。</span><span class="sxs-lookup"><span data-stu-id="d3aea-146">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="d3aea-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3aea-147">createdDateTime</span></span>|<span data-ttu-id="d3aea-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3aea-148">DateTimeOffset</span></span>|<span data-ttu-id="d3aea-149">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="d3aea-149">The date time that the profile was created.</span></span>|
|<span data-ttu-id="d3aea-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3aea-150">lastModifiedDateTime</span></span>|<span data-ttu-id="d3aea-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3aea-151">DateTimeOffset</span></span>|<span data-ttu-id="d3aea-152">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="d3aea-152">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="d3aea-153">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d3aea-153">roleScopeTagIds</span></span>|<span data-ttu-id="d3aea-154">String collection</span><span class="sxs-lookup"><span data-stu-id="d3aea-154">String collection</span></span>|<span data-ttu-id="d3aea-155">此功能更新实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d3aea-155">List of Scope Tags for this Feature Update entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3aea-156">关系</span><span class="sxs-lookup"><span data-stu-id="d3aea-156">Relationships</span></span>
|<span data-ttu-id="d3aea-157">关系</span><span class="sxs-lookup"><span data-stu-id="d3aea-157">Relationship</span></span>|<span data-ttu-id="d3aea-158">类型</span><span class="sxs-lookup"><span data-stu-id="d3aea-158">Type</span></span>|<span data-ttu-id="d3aea-159">说明</span><span class="sxs-lookup"><span data-stu-id="d3aea-159">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3aea-160">assignments</span><span class="sxs-lookup"><span data-stu-id="d3aea-160">assignments</span></span>|<span data-ttu-id="d3aea-161">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3aea-161">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="d3aea-162">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="d3aea-162">The list of group assignments of the profile.</span></span>|
|<span data-ttu-id="d3aea-163">deviceUpdateStates</span><span class="sxs-lookup"><span data-stu-id="d3aea-163">deviceUpdateStates</span></span>|<span data-ttu-id="d3aea-164">[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d3aea-164">[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) collection</span></span>|<span data-ttu-id="d3aea-165">此配置文件指向的设备状态的列表</span><span class="sxs-lookup"><span data-stu-id="d3aea-165">The list of device states this profile targeted to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3aea-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3aea-166">JSON Representation</span></span>
<span data-ttu-id="d3aea-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3aea-167">Here is a JSON representation of the resource.</span></span>
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
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```





