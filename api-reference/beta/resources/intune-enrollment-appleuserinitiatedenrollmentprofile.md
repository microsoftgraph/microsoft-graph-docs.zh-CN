---
title: appleUserInitiatedEnrollmentProfile 资源类型
description: EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b6bf6eefeb94156b85affa3df72665fbe4c3f7bb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783569"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="5197b-104">appleUserInitiatedEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="5197b-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

> <span data-ttu-id="5197b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5197b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5197b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5197b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5197b-107">EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。</span><span class="sxs-lookup"><span data-stu-id="5197b-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="5197b-108">预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="5197b-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="5197b-109">方法</span><span class="sxs-lookup"><span data-stu-id="5197b-109">Methods</span></span>
|<span data-ttu-id="5197b-110">方法</span><span class="sxs-lookup"><span data-stu-id="5197b-110">Method</span></span>|<span data-ttu-id="5197b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="5197b-111">Return Type</span></span>|<span data-ttu-id="5197b-112">说明</span><span class="sxs-lookup"><span data-stu-id="5197b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5197b-113">列出 appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="5197b-113">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="5197b-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="5197b-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="5197b-115">列出[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5197b-115">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="5197b-116">获取 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-116">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="5197b-117">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-117">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="5197b-118">读取[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5197b-118">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5197b-119">创建 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-119">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="5197b-120">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-120">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="5197b-121">创建新的[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5197b-121">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5197b-122">删除 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-122">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="5197b-123">None</span><span class="sxs-lookup"><span data-stu-id="5197b-123">None</span></span>|<span data-ttu-id="5197b-124">删除[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="5197b-124">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="5197b-125">更新 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-125">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="5197b-126">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5197b-126">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="5197b-127">更新[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5197b-127">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="5197b-128">setPriority action</span><span class="sxs-lookup"><span data-stu-id="5197b-128">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="5197b-129">无</span><span class="sxs-lookup"><span data-stu-id="5197b-129">None</span></span>|<span data-ttu-id="5197b-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5197b-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5197b-131">属性</span><span class="sxs-lookup"><span data-stu-id="5197b-131">Properties</span></span>
|<span data-ttu-id="5197b-132">属性</span><span class="sxs-lookup"><span data-stu-id="5197b-132">Property</span></span>|<span data-ttu-id="5197b-133">类型</span><span class="sxs-lookup"><span data-stu-id="5197b-133">Type</span></span>|<span data-ttu-id="5197b-134">说明</span><span class="sxs-lookup"><span data-stu-id="5197b-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5197b-135">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5197b-135">defaultEnrollmentType</span></span>|[<span data-ttu-id="5197b-136">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5197b-136">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="5197b-137">默认配置文件注册类型。</span><span class="sxs-lookup"><span data-stu-id="5197b-137">The default profile enrollment type.</span></span> <span data-ttu-id="5197b-138">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="5197b-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="5197b-139">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="5197b-139">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="5197b-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)集合</span><span class="sxs-lookup"><span data-stu-id="5197b-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="5197b-141">可用注册类型选项的列表</span><span class="sxs-lookup"><span data-stu-id="5197b-141">List of available enrollment type options</span></span>|
|<span data-ttu-id="5197b-142">id</span><span class="sxs-lookup"><span data-stu-id="5197b-142">id</span></span>|<span data-ttu-id="5197b-143">字符串</span><span class="sxs-lookup"><span data-stu-id="5197b-143">String</span></span>|<span data-ttu-id="5197b-144">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="5197b-144">The GUID for the object</span></span>|
|<span data-ttu-id="5197b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5197b-145">displayName</span></span>|<span data-ttu-id="5197b-146">String</span><span class="sxs-lookup"><span data-stu-id="5197b-146">String</span></span>|<span data-ttu-id="5197b-147">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="5197b-147">Name of the profile</span></span>|
|<span data-ttu-id="5197b-148">说明</span><span class="sxs-lookup"><span data-stu-id="5197b-148">description</span></span>|<span data-ttu-id="5197b-149">String</span><span class="sxs-lookup"><span data-stu-id="5197b-149">String</span></span>|<span data-ttu-id="5197b-150">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="5197b-150">Description of the profile</span></span>|
|<span data-ttu-id="5197b-151">priority</span><span class="sxs-lookup"><span data-stu-id="5197b-151">priority</span></span>|<span data-ttu-id="5197b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5197b-152">Int32</span></span>|<span data-ttu-id="5197b-153">优先级，0为最高</span><span class="sxs-lookup"><span data-stu-id="5197b-153">Priority, 0 is highest</span></span>|
|<span data-ttu-id="5197b-154">platform</span><span class="sxs-lookup"><span data-stu-id="5197b-154">platform</span></span>|[<span data-ttu-id="5197b-155">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="5197b-155">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="5197b-156">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="5197b-156">The platform of the Device.</span></span> <span data-ttu-id="5197b-157">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="5197b-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="5197b-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5197b-158">createdDateTime</span></span>|<span data-ttu-id="5197b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5197b-159">DateTimeOffset</span></span>|<span data-ttu-id="5197b-160">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="5197b-160">Profile creation time</span></span>|
|<span data-ttu-id="5197b-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5197b-161">lastModifiedDateTime</span></span>|<span data-ttu-id="5197b-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5197b-162">DateTimeOffset</span></span>|<span data-ttu-id="5197b-163">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="5197b-163">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="5197b-164">关系</span><span class="sxs-lookup"><span data-stu-id="5197b-164">Relationships</span></span>
|<span data-ttu-id="5197b-165">关系</span><span class="sxs-lookup"><span data-stu-id="5197b-165">Relationship</span></span>|<span data-ttu-id="5197b-166">类型</span><span class="sxs-lookup"><span data-stu-id="5197b-166">Type</span></span>|<span data-ttu-id="5197b-167">说明</span><span class="sxs-lookup"><span data-stu-id="5197b-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5197b-168">assignments</span><span class="sxs-lookup"><span data-stu-id="5197b-168">assignments</span></span>|<span data-ttu-id="5197b-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="5197b-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="5197b-170">此配置文件的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="5197b-170">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5197b-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5197b-171">JSON Representation</span></span>
<span data-ttu-id="5197b-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5197b-172">Here is a JSON representation of the resource.</span></span>
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



