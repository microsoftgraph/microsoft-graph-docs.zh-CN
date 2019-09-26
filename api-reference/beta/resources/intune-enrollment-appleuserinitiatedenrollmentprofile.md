---
title: appleUserInitiatedEnrollmentProfile 资源类型
description: EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。 预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed568d5d8169623b5ff3e006d22cdfe5cecd4a47
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199988"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="a97f0-104">appleUserInitiatedEnrollmentProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a97f0-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

> <span data-ttu-id="a97f0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a97f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a97f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a97f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a97f0-107">EnrollmentProfile 资源表示必须提供预注册的配置的集合，以便能够注册已预暂存其标识的某些设备。</span><span class="sxs-lookup"><span data-stu-id="a97f0-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="a97f0-108">预暂存的设备标识分配给此类型的配置文件，以便在注册相应设备时应用配置文件的配置。</span><span class="sxs-lookup"><span data-stu-id="a97f0-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="a97f0-109">方法</span><span class="sxs-lookup"><span data-stu-id="a97f0-109">Methods</span></span>
|<span data-ttu-id="a97f0-110">方法</span><span class="sxs-lookup"><span data-stu-id="a97f0-110">Method</span></span>|<span data-ttu-id="a97f0-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="a97f0-111">Return Type</span></span>|<span data-ttu-id="a97f0-112">说明</span><span class="sxs-lookup"><span data-stu-id="a97f0-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a97f0-113">列出 appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="a97f0-113">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="a97f0-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)集合</span><span class="sxs-lookup"><span data-stu-id="a97f0-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="a97f0-115">列出[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a97f0-115">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="a97f0-116">获取 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-116">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="a97f0-117">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-117">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="a97f0-118">读取[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a97f0-118">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="a97f0-119">创建 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-119">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="a97f0-120">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-120">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="a97f0-121">创建新的[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a97f0-121">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="a97f0-122">删除 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-122">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="a97f0-123">无</span><span class="sxs-lookup"><span data-stu-id="a97f0-123">None</span></span>|<span data-ttu-id="a97f0-124">删除[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="a97f0-124">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="a97f0-125">更新 appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-125">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="a97f0-126">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a97f0-126">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="a97f0-127">更新[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a97f0-127">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="a97f0-128">setPriority action</span><span class="sxs-lookup"><span data-stu-id="a97f0-128">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="a97f0-129">无</span><span class="sxs-lookup"><span data-stu-id="a97f0-129">None</span></span>|<span data-ttu-id="a97f0-130">尚未记录</span><span class="sxs-lookup"><span data-stu-id="a97f0-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a97f0-131">属性</span><span class="sxs-lookup"><span data-stu-id="a97f0-131">Properties</span></span>
|<span data-ttu-id="a97f0-132">属性</span><span class="sxs-lookup"><span data-stu-id="a97f0-132">Property</span></span>|<span data-ttu-id="a97f0-133">类型</span><span class="sxs-lookup"><span data-stu-id="a97f0-133">Type</span></span>|<span data-ttu-id="a97f0-134">说明</span><span class="sxs-lookup"><span data-stu-id="a97f0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a97f0-135">defaultEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a97f0-135">defaultEnrollmentType</span></span>|[<span data-ttu-id="a97f0-136">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a97f0-136">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="a97f0-137">默认配置文件注册类型。</span><span class="sxs-lookup"><span data-stu-id="a97f0-137">The default profile enrollment type.</span></span> <span data-ttu-id="a97f0-138">可取值为：`unknown`、`device`、`user`。</span><span class="sxs-lookup"><span data-stu-id="a97f0-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="a97f0-139">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="a97f0-139">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="a97f0-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)集合</span><span class="sxs-lookup"><span data-stu-id="a97f0-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="a97f0-141">可用注册类型选项的列表</span><span class="sxs-lookup"><span data-stu-id="a97f0-141">List of available enrollment type options</span></span>|
|<span data-ttu-id="a97f0-142">id</span><span class="sxs-lookup"><span data-stu-id="a97f0-142">id</span></span>|<span data-ttu-id="a97f0-143">字符串</span><span class="sxs-lookup"><span data-stu-id="a97f0-143">String</span></span>|<span data-ttu-id="a97f0-144">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="a97f0-144">The GUID for the object</span></span>|
|<span data-ttu-id="a97f0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a97f0-145">displayName</span></span>|<span data-ttu-id="a97f0-146">String</span><span class="sxs-lookup"><span data-stu-id="a97f0-146">String</span></span>|<span data-ttu-id="a97f0-147">配置文件的名称</span><span class="sxs-lookup"><span data-stu-id="a97f0-147">Name of the profile</span></span>|
|<span data-ttu-id="a97f0-148">说明</span><span class="sxs-lookup"><span data-stu-id="a97f0-148">description</span></span>|<span data-ttu-id="a97f0-149">String</span><span class="sxs-lookup"><span data-stu-id="a97f0-149">String</span></span>|<span data-ttu-id="a97f0-150">配置文件的说明</span><span class="sxs-lookup"><span data-stu-id="a97f0-150">Description of the profile</span></span>|
|<span data-ttu-id="a97f0-151">priority</span><span class="sxs-lookup"><span data-stu-id="a97f0-151">priority</span></span>|<span data-ttu-id="a97f0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a97f0-152">Int32</span></span>|<span data-ttu-id="a97f0-153">优先级，0为最高</span><span class="sxs-lookup"><span data-stu-id="a97f0-153">Priority, 0 is highest</span></span>|
|<span data-ttu-id="a97f0-154">platform</span><span class="sxs-lookup"><span data-stu-id="a97f0-154">platform</span></span>|[<span data-ttu-id="a97f0-155">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="a97f0-155">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="a97f0-156">设备的平台。</span><span class="sxs-lookup"><span data-stu-id="a97f0-156">The platform of the Device.</span></span> <span data-ttu-id="a97f0-157">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="a97f0-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="a97f0-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a97f0-158">createdDateTime</span></span>|<span data-ttu-id="a97f0-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a97f0-159">DateTimeOffset</span></span>|<span data-ttu-id="a97f0-160">配置文件创建时间</span><span class="sxs-lookup"><span data-stu-id="a97f0-160">Profile creation time</span></span>|
|<span data-ttu-id="a97f0-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a97f0-161">lastModifiedDateTime</span></span>|<span data-ttu-id="a97f0-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a97f0-162">DateTimeOffset</span></span>|<span data-ttu-id="a97f0-163">配置文件上次修改时间</span><span class="sxs-lookup"><span data-stu-id="a97f0-163">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="a97f0-164">关系</span><span class="sxs-lookup"><span data-stu-id="a97f0-164">Relationships</span></span>
|<span data-ttu-id="a97f0-165">关系</span><span class="sxs-lookup"><span data-stu-id="a97f0-165">Relationship</span></span>|<span data-ttu-id="a97f0-166">类型</span><span class="sxs-lookup"><span data-stu-id="a97f0-166">Type</span></span>|<span data-ttu-id="a97f0-167">说明</span><span class="sxs-lookup"><span data-stu-id="a97f0-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a97f0-168">assignments</span><span class="sxs-lookup"><span data-stu-id="a97f0-168">assignments</span></span>|<span data-ttu-id="a97f0-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="a97f0-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="a97f0-170">此配置文件的工作分配列表。</span><span class="sxs-lookup"><span data-stu-id="a97f0-170">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a97f0-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a97f0-171">JSON Representation</span></span>
<span data-ttu-id="a97f0-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a97f0-172">Here is a JSON representation of the resource.</span></span>
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



