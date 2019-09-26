---
title: windowsFeatureUpdateProfile 资源类型
description: Windows 功能更新配置文件
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4806f33f753560739c9ced128c64d3a626b9b03a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199893"
---
# <a name="windowsfeatureupdateprofile-resource-type"></a><span data-ttu-id="62f16-103">windowsFeatureUpdateProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="62f16-103">windowsFeatureUpdateProfile resource type</span></span>

> <span data-ttu-id="62f16-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62f16-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62f16-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62f16-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62f16-106">Windows 功能更新配置文件</span><span class="sxs-lookup"><span data-stu-id="62f16-106">Windows Feature Update Profile</span></span>

## <a name="methods"></a><span data-ttu-id="62f16-107">方法</span><span class="sxs-lookup"><span data-stu-id="62f16-107">Methods</span></span>
|<span data-ttu-id="62f16-108">方法</span><span class="sxs-lookup"><span data-stu-id="62f16-108">Method</span></span>|<span data-ttu-id="62f16-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="62f16-109">Return Type</span></span>|<span data-ttu-id="62f16-110">说明</span><span class="sxs-lookup"><span data-stu-id="62f16-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="62f16-111">列出 windowsFeatureUpdateProfiles</span><span class="sxs-lookup"><span data-stu-id="62f16-111">List windowsFeatureUpdateProfiles</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-list.md)|<span data-ttu-id="62f16-112">[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="62f16-112">[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) collection</span></span>|<span data-ttu-id="62f16-113">列出[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62f16-113">List properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) objects.</span></span>|
|[<span data-ttu-id="62f16-114">获取 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-114">Get windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-get.md)|[<span data-ttu-id="62f16-115">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-115">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="62f16-116">读取[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="62f16-116">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="62f16-117">创建 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-117">Create windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-create.md)|[<span data-ttu-id="62f16-118">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-118">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="62f16-119">创建新的[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62f16-119">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="62f16-120">删除 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-120">Delete windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-delete.md)|<span data-ttu-id="62f16-121">无</span><span class="sxs-lookup"><span data-stu-id="62f16-121">None</span></span>|<span data-ttu-id="62f16-122">删除[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="62f16-122">Deletes a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>|
|[<span data-ttu-id="62f16-123">更新 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-123">Update windowsFeatureUpdateProfile</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-update.md)|[<span data-ttu-id="62f16-124">windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="62f16-124">windowsFeatureUpdateProfile</span></span>](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)|<span data-ttu-id="62f16-125">更新[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="62f16-125">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>|
|[<span data-ttu-id="62f16-126">分配操作</span><span class="sxs-lookup"><span data-stu-id="62f16-126">assign action</span></span>](../api/intune-softwareupdate-windowsfeatureupdateprofile-assign.md)|<span data-ttu-id="62f16-127">无</span><span class="sxs-lookup"><span data-stu-id="62f16-127">None</span></span>|<span data-ttu-id="62f16-128">尚未记录</span><span class="sxs-lookup"><span data-stu-id="62f16-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="62f16-129">属性</span><span class="sxs-lookup"><span data-stu-id="62f16-129">Properties</span></span>
|<span data-ttu-id="62f16-130">属性</span><span class="sxs-lookup"><span data-stu-id="62f16-130">Property</span></span>|<span data-ttu-id="62f16-131">类型</span><span class="sxs-lookup"><span data-stu-id="62f16-131">Type</span></span>|<span data-ttu-id="62f16-132">说明</span><span class="sxs-lookup"><span data-stu-id="62f16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f16-133">id</span><span class="sxs-lookup"><span data-stu-id="62f16-133">id</span></span>|<span data-ttu-id="62f16-134">字符串</span><span class="sxs-lookup"><span data-stu-id="62f16-134">String</span></span>|<span data-ttu-id="62f16-135">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="62f16-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="62f16-136">displayName</span><span class="sxs-lookup"><span data-stu-id="62f16-136">displayName</span></span>|<span data-ttu-id="62f16-137">String</span><span class="sxs-lookup"><span data-stu-id="62f16-137">String</span></span>|<span data-ttu-id="62f16-138">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="62f16-138">The display name of the profile.</span></span>|
|<span data-ttu-id="62f16-139">说明</span><span class="sxs-lookup"><span data-stu-id="62f16-139">description</span></span>|<span data-ttu-id="62f16-140">String</span><span class="sxs-lookup"><span data-stu-id="62f16-140">String</span></span>|<span data-ttu-id="62f16-141">用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="62f16-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="62f16-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="62f16-142">featureUpdateVersion</span></span>|<span data-ttu-id="62f16-143">String</span><span class="sxs-lookup"><span data-stu-id="62f16-143">String</span></span>|<span data-ttu-id="62f16-144">将部署到此配置文件目标的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="62f16-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="62f16-145">版本可以是任何受支持的版本，例如，1709、1803或1809等。</span><span class="sxs-lookup"><span data-stu-id="62f16-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="62f16-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62f16-146">createdDateTime</span></span>|<span data-ttu-id="62f16-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62f16-147">DateTimeOffset</span></span>|<span data-ttu-id="62f16-148">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="62f16-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="62f16-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62f16-149">lastModifiedDateTime</span></span>|<span data-ttu-id="62f16-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62f16-150">DateTimeOffset</span></span>|<span data-ttu-id="62f16-151">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="62f16-151">The date time that the profile was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62f16-152">关系</span><span class="sxs-lookup"><span data-stu-id="62f16-152">Relationships</span></span>
|<span data-ttu-id="62f16-153">关系</span><span class="sxs-lookup"><span data-stu-id="62f16-153">Relationship</span></span>|<span data-ttu-id="62f16-154">类型</span><span class="sxs-lookup"><span data-stu-id="62f16-154">Type</span></span>|<span data-ttu-id="62f16-155">说明</span><span class="sxs-lookup"><span data-stu-id="62f16-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f16-156">assignments</span><span class="sxs-lookup"><span data-stu-id="62f16-156">assignments</span></span>|<span data-ttu-id="62f16-157">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="62f16-157">[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) collection</span></span>|<span data-ttu-id="62f16-158">配置文件的组分配列表。</span><span class="sxs-lookup"><span data-stu-id="62f16-158">The list of group assignments of the profile.</span></span>|
|<span data-ttu-id="62f16-159">deviceUpdateStates</span><span class="sxs-lookup"><span data-stu-id="62f16-159">deviceUpdateStates</span></span>|<span data-ttu-id="62f16-160">[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="62f16-160">[windowsUpdateState](../resources/intune-shared-windowsupdatestate.md) collection</span></span>|<span data-ttu-id="62f16-161">此配置文件指向的设备状态的列表</span><span class="sxs-lookup"><span data-stu-id="62f16-161">The list of device states this profile targeted to</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62f16-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62f16-162">JSON Representation</span></span>
<span data-ttu-id="62f16-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62f16-163">Here is a JSON representation of the resource.</span></span>
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



