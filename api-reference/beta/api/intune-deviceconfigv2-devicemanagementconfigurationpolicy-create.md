---
title: 创建 deviceManagementConfigurationPolicy
description: 创建新的 deviceManagementConfigurationPolicy 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 044059bddb9893fb4c7f2520a56d1774f6b47792
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241502"
---
# <a name="create-devicemanagementconfigurationpolicy"></a><span data-ttu-id="a0d20-103">创建 deviceManagementConfigurationPolicy</span><span class="sxs-lookup"><span data-stu-id="a0d20-103">Create deviceManagementConfigurationPolicy</span></span>

<span data-ttu-id="a0d20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0d20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0d20-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0d20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0d20-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0d20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0d20-107">创建新的 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0d20-107">Create a new [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0d20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0d20-108">Prerequisites</span></span>
<span data-ttu-id="a0d20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0d20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0d20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0d20-111">Permission type</span></span>|<span data-ttu-id="a0d20-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a0d20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0d20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0d20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0d20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0d20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0d20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0d20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0d20-116">Not supported.</span></span>|
|<span data-ttu-id="a0d20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0d20-117">Application</span></span>|<span data-ttu-id="a0d20-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0d20-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0d20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0d20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configurationPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a0d20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0d20-120">Request headers</span></span>
|<span data-ttu-id="a0d20-121">标头</span><span class="sxs-lookup"><span data-stu-id="a0d20-121">Header</span></span>|<span data-ttu-id="a0d20-122">值</span><span class="sxs-lookup"><span data-stu-id="a0d20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0d20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0d20-123">Authorization</span></span>|<span data-ttu-id="a0d20-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0d20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0d20-125">接受</span><span class="sxs-lookup"><span data-stu-id="a0d20-125">Accept</span></span>|<span data-ttu-id="a0d20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0d20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0d20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0d20-127">Request body</span></span>
<span data-ttu-id="a0d20-128">在请求正文中，提供 deviceManagementConfigurationPolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0d20-128">In the request body, supply a JSON representation for the deviceManagementConfigurationPolicy object.</span></span>

<span data-ttu-id="a0d20-129">下表显示创建 deviceManagementConfigurationPolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0d20-129">The following table shows the properties that are required when you create the deviceManagementConfigurationPolicy.</span></span>

|<span data-ttu-id="a0d20-130">属性</span><span class="sxs-lookup"><span data-stu-id="a0d20-130">Property</span></span>|<span data-ttu-id="a0d20-131">类型</span><span class="sxs-lookup"><span data-stu-id="a0d20-131">Type</span></span>|<span data-ttu-id="a0d20-132">说明</span><span class="sxs-lookup"><span data-stu-id="a0d20-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0d20-133">id</span><span class="sxs-lookup"><span data-stu-id="a0d20-133">id</span></span>|<span data-ttu-id="a0d20-134">String</span><span class="sxs-lookup"><span data-stu-id="a0d20-134">String</span></span>|<span data-ttu-id="a0d20-135">策略文档的键。</span><span class="sxs-lookup"><span data-stu-id="a0d20-135">Key of the policy document.</span></span> <span data-ttu-id="a0d20-136">自动生成。</span><span class="sxs-lookup"><span data-stu-id="a0d20-136">Automatically generated.</span></span>|
|<span data-ttu-id="a0d20-137">name</span><span class="sxs-lookup"><span data-stu-id="a0d20-137">name</span></span>|<span data-ttu-id="a0d20-138">String</span><span class="sxs-lookup"><span data-stu-id="a0d20-138">String</span></span>|<span data-ttu-id="a0d20-139">策略名称</span><span class="sxs-lookup"><span data-stu-id="a0d20-139">Policy name</span></span>|
|<span data-ttu-id="a0d20-140">description</span><span class="sxs-lookup"><span data-stu-id="a0d20-140">description</span></span>|<span data-ttu-id="a0d20-141">String</span><span class="sxs-lookup"><span data-stu-id="a0d20-141">String</span></span>|<span data-ttu-id="a0d20-142">策略说明</span><span class="sxs-lookup"><span data-stu-id="a0d20-142">Policy description</span></span>|
|<span data-ttu-id="a0d20-143">平台</span><span class="sxs-lookup"><span data-stu-id="a0d20-143">platforms</span></span>|[<span data-ttu-id="a0d20-144">deviceManagementConfigurationPlatforms</span><span class="sxs-lookup"><span data-stu-id="a0d20-144">deviceManagementConfigurationPlatforms</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationplatforms.md)|<span data-ttu-id="a0d20-145">此策略的平台。</span><span class="sxs-lookup"><span data-stu-id="a0d20-145">Platforms for this policy.</span></span> <span data-ttu-id="a0d20-146">可取值为：`none`、`macOS`、`windows10X`、`windows10`。</span><span class="sxs-lookup"><span data-stu-id="a0d20-146">Possible values are: `none`, `macOS`, `windows10X`, `windows10`.</span></span>|
|<span data-ttu-id="a0d20-147">技术</span><span class="sxs-lookup"><span data-stu-id="a0d20-147">technologies</span></span>|[<span data-ttu-id="a0d20-148">deviceManagementConfigurationTechnologies</span><span class="sxs-lookup"><span data-stu-id="a0d20-148">deviceManagementConfigurationTechnologies</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationtechnologies.md)|<span data-ttu-id="a0d20-149">适用于此策略的技术。</span><span class="sxs-lookup"><span data-stu-id="a0d20-149">Technologies for this policy.</span></span> <span data-ttu-id="a0d20-150">可取值为：`none`、`mdm`、`windows10XManagement`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="a0d20-150">Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`.</span></span>|
|<span data-ttu-id="a0d20-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d20-151">createdDateTime</span></span>|<span data-ttu-id="a0d20-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d20-152">DateTimeOffset</span></span>|<span data-ttu-id="a0d20-153">策略创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0d20-153">Policy creation date and time.</span></span> <span data-ttu-id="a0d20-154">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a0d20-154">This property is read-only.</span></span>|
|<span data-ttu-id="a0d20-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0d20-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a0d20-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0d20-156">DateTimeOffset</span></span>|<span data-ttu-id="a0d20-157">策略上次修改日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a0d20-157">Policy last modification date and time.</span></span> <span data-ttu-id="a0d20-158">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a0d20-158">This property is read-only.</span></span>|
|<span data-ttu-id="a0d20-159">settingCount</span><span class="sxs-lookup"><span data-stu-id="a0d20-159">settingCount</span></span>|<span data-ttu-id="a0d20-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a0d20-160">Int32</span></span>|<span data-ttu-id="a0d20-161">设置的数目。</span><span class="sxs-lookup"><span data-stu-id="a0d20-161">Number of settings.</span></span> <span data-ttu-id="a0d20-162">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a0d20-162">This property is read-only.</span></span>|
|<span data-ttu-id="a0d20-163">creationSource</span><span class="sxs-lookup"><span data-stu-id="a0d20-163">creationSource</span></span>|<span data-ttu-id="a0d20-164">String</span><span class="sxs-lookup"><span data-stu-id="a0d20-164">String</span></span>|<span data-ttu-id="a0d20-165">策略创建源</span><span class="sxs-lookup"><span data-stu-id="a0d20-165">Policy creation source</span></span>|
|<span data-ttu-id="a0d20-166">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0d20-166">roleScopeTagIds</span></span>|<span data-ttu-id="a0d20-167">String 集合</span><span class="sxs-lookup"><span data-stu-id="a0d20-167">String collection</span></span>|<span data-ttu-id="a0d20-168">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a0d20-168">List of Scope Tags for this Entity instance.</span></span>|
|<span data-ttu-id="a0d20-169">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a0d20-169">isAssigned</span></span>|<span data-ttu-id="a0d20-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0d20-170">Boolean</span></span>|<span data-ttu-id="a0d20-171">策略分配状态。</span><span class="sxs-lookup"><span data-stu-id="a0d20-171">Policy assignment status.</span></span> <span data-ttu-id="a0d20-172">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a0d20-172">This property is read-only.</span></span>|



## <a name="response"></a><span data-ttu-id="a0d20-173">响应</span><span class="sxs-lookup"><span data-stu-id="a0d20-173">Response</span></span>
<span data-ttu-id="a0d20-174">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0d20-174">If successful, this method returns a `201 Created` response code and a [deviceManagementConfigurationPolicy](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0d20-175">示例</span><span class="sxs-lookup"><span data-stu-id="a0d20-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0d20-176">请求</span><span class="sxs-lookup"><span data-stu-id="a0d20-176">Request</span></span>
<span data-ttu-id="a0d20-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0d20-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configurationPolicies
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

### <a name="response"></a><span data-ttu-id="a0d20-178">响应</span><span class="sxs-lookup"><span data-stu-id="a0d20-178">Response</span></span>
<span data-ttu-id="a0d20-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0d20-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




