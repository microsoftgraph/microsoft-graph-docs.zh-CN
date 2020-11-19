---
title: 更新 deviceManagementConfigurationPolicy
description: 更新 deviceManagementConfigurationPolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cc4ba12c9c989f1066d7ce690135f4fc5499479
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241497"
---
# <a name="update-devicemanagementconfigurationpolicy"></a><span data-ttu-id="92aa4-103">更新 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="92aa4-103">Update deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="92aa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92aa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92aa4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92aa4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92aa4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92aa4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92aa4-107">更新 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="92aa4-107">Update the properties of a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92aa4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="92aa4-108">Prerequisites</span></span>
<span data-ttu-id="92aa4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92aa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92aa4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="92aa4-111">Permission type</span></span>|<span data-ttu-id="92aa4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="92aa4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92aa4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92aa4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92aa4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92aa4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92aa4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92aa4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92aa4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="92aa4-116">Not supported.</span></span>|
|<span data-ttu-id="92aa4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="92aa4-117">Application</span></span>|<span data-ttu-id="92aa4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92aa4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92aa4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92aa4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="92aa4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="92aa4-120">Request headers</span></span>
|<span data-ttu-id="92aa4-121">标头</span><span class="sxs-lookup"><span data-stu-id="92aa4-121">Header</span></span>|<span data-ttu-id="92aa4-122">值</span><span class="sxs-lookup"><span data-stu-id="92aa4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92aa4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92aa4-123">Authorization</span></span>|<span data-ttu-id="92aa4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="92aa4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92aa4-125">接受</span><span class="sxs-lookup"><span data-stu-id="92aa4-125">Accept</span></span>|<span data-ttu-id="92aa4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92aa4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92aa4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="92aa4-127">Request body</span></span>
<span data-ttu-id="92aa4-128">在请求正文中，提供 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92aa4-128">In the request body, supply a JSON representation for the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

<span data-ttu-id="92aa4-129">下表显示创建 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="92aa4-129">The following table shows the properties that are required when you create the [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md).</span></span>

|<span data-ttu-id="92aa4-130">属性</span><span class="sxs-lookup"><span data-stu-id="92aa4-130">Property</span></span>|<span data-ttu-id="92aa4-131">类型</span><span class="sxs-lookup"><span data-stu-id="92aa4-131">Type</span></span>|<span data-ttu-id="92aa4-132">说明</span><span class="sxs-lookup"><span data-stu-id="92aa4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92aa4-133">id</span><span class="sxs-lookup"><span data-stu-id="92aa4-133">id</span></span>|<span data-ttu-id="92aa4-134">String</span><span class="sxs-lookup"><span data-stu-id="92aa4-134">String</span></span>|<span data-ttu-id="92aa4-135">策略文档的键。</span><span class="sxs-lookup"><span data-stu-id="92aa4-135">Key of the policy document.</span></span> <span data-ttu-id="92aa4-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="92aa4-136">Automatically generated.</span></span>|
|<span data-ttu-id="92aa4-137">name</span><span class="sxs-lookup"><span data-stu-id="92aa4-137">name</span></span>|<span data-ttu-id="92aa4-138">String</span><span class="sxs-lookup"><span data-stu-id="92aa4-138">String</span></span>|<span data-ttu-id="92aa4-139">策略名称</span><span class="sxs-lookup"><span data-stu-id="92aa4-139">Policy name</span></span>|
|<span data-ttu-id="92aa4-140">description</span><span class="sxs-lookup"><span data-stu-id="92aa4-140">description</span></span>|<span data-ttu-id="92aa4-141">String</span><span class="sxs-lookup"><span data-stu-id="92aa4-141">String</span></span>|<span data-ttu-id="92aa4-142">策略说明</span><span class="sxs-lookup"><span data-stu-id="92aa4-142">Policy description</span></span>|
|<span data-ttu-id="92aa4-143">平台</span><span class="sxs-lookup"><span data-stu-id="92aa4-143">platforms</span></span>|[<span data-ttu-id="92aa4-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="92aa4-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="92aa4-145">此策略的平台。</span><span class="sxs-lookup"><span data-stu-id="92aa4-145">Platforms for this policy.</span></span> <span data-ttu-id="92aa4-146">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="92aa4-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="92aa4-147">技术</span><span class="sxs-lookup"><span data-stu-id="92aa4-147">technologies</span></span>|[<span data-ttu-id="92aa4-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="92aa4-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="92aa4-149">适用于此策略的技术。</span><span class="sxs-lookup"><span data-stu-id="92aa4-149">Technologies for this policy.</span></span> <span data-ttu-id="92aa4-150">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="92aa4-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="92aa4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92aa4-151">createdDateTime</span></span>|<span data-ttu-id="92aa4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92aa4-152">DateTimeOffset</span></span>|<span data-ttu-id="92aa4-153">策略创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="92aa4-153">Policy creation date and time.</span></span> <span data-ttu-id="92aa4-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="92aa4-154">This property is read-only.</span></span>|
|<span data-ttu-id="92aa4-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92aa4-155">lastModifiedDateTime</span></span>|<span data-ttu-id="92aa4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92aa4-156">DateTimeOffset</span></span>|<span data-ttu-id="92aa4-157">策略上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="92aa4-157">Policy last modification date and time.</span></span> <span data-ttu-id="92aa4-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="92aa4-158">This property is read-only.</span></span>|
|<span data-ttu-id="92aa4-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="92aa4-159">settingCount</span></span>|<span data-ttu-id="92aa4-160">Int32</span><span class="sxs-lookup"><span data-stu-id="92aa4-160">Int32</span></span>|<span data-ttu-id="92aa4-161">设置的数目。</span><span class="sxs-lookup"><span data-stu-id="92aa4-161">Number of settings.</span></span> <span data-ttu-id="92aa4-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="92aa4-162">This property is read-only.</span></span>|
|<span data-ttu-id="92aa4-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="92aa4-163">creationSource</span></span>|<span data-ttu-id="92aa4-164">String</span><span class="sxs-lookup"><span data-stu-id="92aa4-164">String</span></span>|<span data-ttu-id="92aa4-165">策略创建源</span><span class="sxs-lookup"><span data-stu-id="92aa4-165">Policy creation source</span></span>|
|<span data-ttu-id="92aa4-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92aa4-166">roleScopeTagIds</span></span>|<span data-ttu-id="92aa4-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="92aa4-167">String collection</span></span>|<span data-ttu-id="92aa4-168">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="92aa4-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="92aa4-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="92aa4-169">isAssigned</span></span>|<span data-ttu-id="92aa4-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="92aa4-170">Boolean</span></span>|<span data-ttu-id="92aa4-171">策略分配状态。</span><span class="sxs-lookup"><span data-stu-id="92aa4-171">Policy assignment status.</span></span> <span data-ttu-id="92aa4-172">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="92aa4-172">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="92aa4-173">响应</span><span class="sxs-lookup"><span data-stu-id="92aa4-173">Response</span></span>
<span data-ttu-id="92aa4-174">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92aa4-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92aa4-175">示例</span><span class="sxs-lookup"><span data-stu-id="92aa4-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="92aa4-176">请求</span><span class="sxs-lookup"><span data-stu-id="92aa4-176">Request</span></span>
<span data-ttu-id="92aa4-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92aa4-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationPolicies/{deviceManagementConfigurationPolicyId}
Content-type: application/json
Content-length: 346

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="92aa4-178">响应</span><span class="sxs-lookup"><span data-stu-id="92aa4-178">Response</span></span>
<span data-ttu-id="92aa4-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92aa4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicy",
  "id": "3ffd7cd0-7cd0-3ffd-d07c-fd3fd07cfd3f",
  "name": "Name value",
  "description": "Description value",
  "platforms": "macOS",
  "technologies": "mdm",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "settingCount": 12,
  "creationSource": "Creation Source value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isAssigned": true
}
```




