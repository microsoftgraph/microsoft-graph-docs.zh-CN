---
title: appleUserInitiatedEnrollmentProfile 资源类型
description: EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f6f7d28d1c5684793891bc8bee08300f67ebeec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419478"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="69cec-104">appleUserInitiatedEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="69cec-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

<span data-ttu-id="69cec-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69cec-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="69cec-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69cec-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69cec-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69cec-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69cec-108">EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。</span><span class="sxs-lookup"><span data-stu-id="69cec-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="69cec-109">预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="69cec-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="69cec-110">方法</span><span class="sxs-lookup"><span data-stu-id="69cec-110">Methods</span></span>
|<span data-ttu-id="69cec-111">方法</span><span class="sxs-lookup"><span data-stu-id="69cec-111">Method</span></span>|<span data-ttu-id="69cec-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="69cec-112">Return Type</span></span>|<span data-ttu-id="69cec-113">说明</span><span class="sxs-lookup"><span data-stu-id="69cec-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69cec-114">列出 appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="69cec-114">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="69cec-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="69cec-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="69cec-116">列出[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69cec-116">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="69cec-117">获取 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-117">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="69cec-118">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-118">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="69cec-119">读取[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69cec-119">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="69cec-120">创建 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-120">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="69cec-121">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-121">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="69cec-122">创建新的[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="69cec-122">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="69cec-123">删除 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-123">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="69cec-124">无</span><span class="sxs-lookup"><span data-stu-id="69cec-124">None</span></span>|<span data-ttu-id="69cec-125">删除[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="69cec-125">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="69cec-126">更新 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-126">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="69cec-127">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="69cec-127">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="69cec-128">更新[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69cec-128">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="69cec-129">setPriority action</span><span class="sxs-lookup"><span data-stu-id="69cec-129">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="69cec-130">无</span><span class="sxs-lookup"><span data-stu-id="69cec-130">None</span></span>|<span data-ttu-id="69cec-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69cec-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="69cec-132">属性</span><span class="sxs-lookup"><span data-stu-id="69cec-132">Properties</span></span>
|<span data-ttu-id="69cec-133">属性</span><span class="sxs-lookup"><span data-stu-id="69cec-133">Property</span></span>|<span data-ttu-id="69cec-134">类型</span><span class="sxs-lookup"><span data-stu-id="69cec-134">Type</span></span>|<span data-ttu-id="69cec-135">说明</span><span class="sxs-lookup"><span data-stu-id="69cec-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cec-136">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="69cec-136">defaultEnrollmentType</span></span>|[<span data-ttu-id="69cec-137">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="69cec-137">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="69cec-138">默认配置文件注册类型。</span><span class="sxs-lookup"><span data-stu-id="69cec-138">The default profile enrollment type.</span></span> <span data-ttu-id="69cec-139">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="69cec-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="69cec-140">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="69cec-140">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="69cec-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)集合</span><span class="sxs-lookup"><span data-stu-id="69cec-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="69cec-142">可用注册类型选项的列表</span><span class="sxs-lookup"><span data-stu-id="69cec-142">List of available enrollment type options</span></span>|
|<span data-ttu-id="69cec-143">id</span><span class="sxs-lookup"><span data-stu-id="69cec-143">id</span></span>|<span data-ttu-id="69cec-144">字符串</span><span class="sxs-lookup"><span data-stu-id="69cec-144">String</span></span>|<span data-ttu-id="69cec-145">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="69cec-145">The GUID for the object</span></span>|
|<span data-ttu-id="69cec-146">displayName</span><span class="sxs-lookup"><span data-stu-id="69cec-146">displayName</span></span>|<span data-ttu-id="69cec-147">String</span><span class="sxs-lookup"><span data-stu-id="69cec-147">String</span></span>|<span data-ttu-id="69cec-148">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="69cec-148">Name of the profile</span></span>|
|<span data-ttu-id="69cec-149">description</span><span class="sxs-lookup"><span data-stu-id="69cec-149">description</span></span>|<span data-ttu-id="69cec-150">String</span><span class="sxs-lookup"><span data-stu-id="69cec-150">String</span></span>|<span data-ttu-id="69cec-151">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="69cec-151">Description of the profile</span></span>|
|<span data-ttu-id="69cec-152">priority</span><span class="sxs-lookup"><span data-stu-id="69cec-152">priority</span></span>|<span data-ttu-id="69cec-153">Int32</span><span class="sxs-lookup"><span data-stu-id="69cec-153">Int32</span></span>|<span data-ttu-id="69cec-154">优先级，0为最高</span><span class="sxs-lookup"><span data-stu-id="69cec-154">Priority, 0 is highest</span></span>|
|<span data-ttu-id="69cec-155">platform</span><span class="sxs-lookup"><span data-stu-id="69cec-155">platform</span></span>|[<span data-ttu-id="69cec-156">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="69cec-156">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="69cec-157">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="69cec-157">The platform of the Device.</span></span> <span data-ttu-id="69cec-158">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="69cec-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="69cec-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69cec-159">createdDateTime</span></span>|<span data-ttu-id="69cec-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69cec-160">DateTimeOffset</span></span>|<span data-ttu-id="69cec-161">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="69cec-161">Profile creation time</span></span>|
|<span data-ttu-id="69cec-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69cec-162">lastModifiedDateTime</span></span>|<span data-ttu-id="69cec-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69cec-163">DateTimeOffset</span></span>|<span data-ttu-id="69cec-164">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="69cec-164">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="69cec-165">关系</span><span class="sxs-lookup"><span data-stu-id="69cec-165">Relationships</span></span>
|<span data-ttu-id="69cec-166">关系</span><span class="sxs-lookup"><span data-stu-id="69cec-166">Relationship</span></span>|<span data-ttu-id="69cec-167">类型</span><span class="sxs-lookup"><span data-stu-id="69cec-167">Type</span></span>|<span data-ttu-id="69cec-168">说明</span><span class="sxs-lookup"><span data-stu-id="69cec-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69cec-169">assignments</span><span class="sxs-lookup"><span data-stu-id="69cec-169">assignments</span></span>|<span data-ttu-id="69cec-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="69cec-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="69cec-171">此配置文件的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="69cec-171">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69cec-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69cec-172">JSON Representation</span></span>
<span data-ttu-id="69cec-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69cec-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "String",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "String",
      "enrollmentType": "String"
    }
  ],
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



