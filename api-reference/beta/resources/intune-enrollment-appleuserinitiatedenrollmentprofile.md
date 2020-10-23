---
title: appleUserInitiatedEnrollmentProfile 资源类型
description: EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d9d4733b6b68a3fc1f09ed34d8a4afdf6e3dad3
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726369"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="13cc7-104">appleUserInitiatedEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="13cc7-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

<span data-ttu-id="13cc7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13cc7-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13cc7-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13cc7-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13cc7-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13cc7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13cc7-108">EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。</span><span class="sxs-lookup"><span data-stu-id="13cc7-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="13cc7-109">预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="13cc7-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="13cc7-110">Methods</span><span class="sxs-lookup"><span data-stu-id="13cc7-110">Methods</span></span>
|<span data-ttu-id="13cc7-111">方法</span><span class="sxs-lookup"><span data-stu-id="13cc7-111">Method</span></span>|<span data-ttu-id="13cc7-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="13cc7-112">Return Type</span></span>|<span data-ttu-id="13cc7-113">说明</span><span class="sxs-lookup"><span data-stu-id="13cc7-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13cc7-114">列出 appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="13cc7-114">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="13cc7-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13cc7-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="13cc7-116">列出 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13cc7-116">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="13cc7-117">获取 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-117">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="13cc7-118">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-118">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="13cc7-119">读取 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13cc7-119">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="13cc7-120">创建 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-120">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="13cc7-121">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-121">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="13cc7-122">创建新的 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="13cc7-122">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="13cc7-123">删除 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-123">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="13cc7-124">无</span><span class="sxs-lookup"><span data-stu-id="13cc7-124">None</span></span>|<span data-ttu-id="13cc7-125">删除 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="13cc7-125">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="13cc7-126">更新 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-126">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="13cc7-127">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="13cc7-127">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="13cc7-128">更新 [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="13cc7-128">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="13cc7-129">setPriority action</span><span class="sxs-lookup"><span data-stu-id="13cc7-129">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="13cc7-130">无</span><span class="sxs-lookup"><span data-stu-id="13cc7-130">None</span></span>|<span data-ttu-id="13cc7-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="13cc7-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="13cc7-132">属性</span><span class="sxs-lookup"><span data-stu-id="13cc7-132">Properties</span></span>
|<span data-ttu-id="13cc7-133">属性</span><span class="sxs-lookup"><span data-stu-id="13cc7-133">Property</span></span>|<span data-ttu-id="13cc7-134">类型</span><span class="sxs-lookup"><span data-stu-id="13cc7-134">Type</span></span>|<span data-ttu-id="13cc7-135">说明</span><span class="sxs-lookup"><span data-stu-id="13cc7-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13cc7-136">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13cc7-136">defaultEnrollmentType</span></span>|[<span data-ttu-id="13cc7-137">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13cc7-137">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="13cc7-138">默认配置文件注册类型。</span><span class="sxs-lookup"><span data-stu-id="13cc7-138">The default profile enrollment type.</span></span> <span data-ttu-id="13cc7-139">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="13cc7-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="13cc7-140">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="13cc7-140">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="13cc7-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13cc7-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="13cc7-142">可用注册类型选项的列表</span><span class="sxs-lookup"><span data-stu-id="13cc7-142">List of available enrollment type options</span></span>|
|<span data-ttu-id="13cc7-143">id</span><span class="sxs-lookup"><span data-stu-id="13cc7-143">id</span></span>|<span data-ttu-id="13cc7-144">String</span><span class="sxs-lookup"><span data-stu-id="13cc7-144">String</span></span>|<span data-ttu-id="13cc7-145">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="13cc7-145">The GUID for the object</span></span>|
|<span data-ttu-id="13cc7-146">displayName</span><span class="sxs-lookup"><span data-stu-id="13cc7-146">displayName</span></span>|<span data-ttu-id="13cc7-147">String</span><span class="sxs-lookup"><span data-stu-id="13cc7-147">String</span></span>|<span data-ttu-id="13cc7-148">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="13cc7-148">Name of the profile</span></span>|
|<span data-ttu-id="13cc7-149">说明</span><span class="sxs-lookup"><span data-stu-id="13cc7-149">description</span></span>|<span data-ttu-id="13cc7-150">String</span><span class="sxs-lookup"><span data-stu-id="13cc7-150">String</span></span>|<span data-ttu-id="13cc7-151">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="13cc7-151">Description of the profile</span></span>|
|<span data-ttu-id="13cc7-152">priority</span><span class="sxs-lookup"><span data-stu-id="13cc7-152">priority</span></span>|<span data-ttu-id="13cc7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="13cc7-153">Int32</span></span>|<span data-ttu-id="13cc7-154">优先级，0为最高</span><span class="sxs-lookup"><span data-stu-id="13cc7-154">Priority, 0 is highest</span></span>|
|<span data-ttu-id="13cc7-155">平台</span><span class="sxs-lookup"><span data-stu-id="13cc7-155">platform</span></span>|[<span data-ttu-id="13cc7-156">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="13cc7-156">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="13cc7-157">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="13cc7-157">The platform of the Device.</span></span> <span data-ttu-id="13cc7-158">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="13cc7-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="13cc7-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13cc7-159">createdDateTime</span></span>|<span data-ttu-id="13cc7-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13cc7-160">DateTimeOffset</span></span>|<span data-ttu-id="13cc7-161">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="13cc7-161">Profile creation time</span></span>|
|<span data-ttu-id="13cc7-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="13cc7-162">lastModifiedDateTime</span></span>|<span data-ttu-id="13cc7-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13cc7-163">DateTimeOffset</span></span>|<span data-ttu-id="13cc7-164">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="13cc7-164">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="13cc7-165">关系</span><span class="sxs-lookup"><span data-stu-id="13cc7-165">Relationships</span></span>
|<span data-ttu-id="13cc7-166">关系</span><span class="sxs-lookup"><span data-stu-id="13cc7-166">Relationship</span></span>|<span data-ttu-id="13cc7-167">类型</span><span class="sxs-lookup"><span data-stu-id="13cc7-167">Type</span></span>|<span data-ttu-id="13cc7-168">说明</span><span class="sxs-lookup"><span data-stu-id="13cc7-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13cc7-169">assignments</span><span class="sxs-lookup"><span data-stu-id="13cc7-169">assignments</span></span>|<span data-ttu-id="13cc7-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13cc7-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="13cc7-171">此配置文件的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="13cc7-171">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13cc7-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13cc7-172">JSON Representation</span></span>
<span data-ttu-id="13cc7-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13cc7-173">Here is a JSON representation of the resource.</span></span>
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





