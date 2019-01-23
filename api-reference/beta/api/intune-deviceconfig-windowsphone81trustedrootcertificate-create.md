---
title: 创建 windowsPhone81TrustedRootCertificate
description: 创建新的 windowsPhone81TrustedRootCertificate 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbabf0ad844712aab587e62830f0fc3654db19d4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417292"
---
# <a name="create-windowsphone81trustedrootcertificate"></a><span data-ttu-id="207ef-103">创建 windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="207ef-103">Create windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="207ef-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="207ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="207ef-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="207ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="207ef-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="207ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="207ef-107">创建新的[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="207ef-107">Create a new [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="207ef-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="207ef-108">Prerequisites</span></span>
<span data-ttu-id="207ef-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="207ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="207ef-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="207ef-111">Permission type</span></span>|<span data-ttu-id="207ef-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="207ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="207ef-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="207ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="207ef-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="207ef-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="207ef-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="207ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="207ef-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="207ef-116">Not supported.</span></span>|
|<span data-ttu-id="207ef-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="207ef-117">Application</span></span>|<span data-ttu-id="207ef-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="207ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="207ef-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="207ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="207ef-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="207ef-120">Request headers</span></span>
|<span data-ttu-id="207ef-121">标头</span><span class="sxs-lookup"><span data-stu-id="207ef-121">Header</span></span>|<span data-ttu-id="207ef-122">值</span><span class="sxs-lookup"><span data-stu-id="207ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="207ef-123">授权</span><span class="sxs-lookup"><span data-stu-id="207ef-123">Authorization</span></span>|<span data-ttu-id="207ef-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="207ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="207ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="207ef-125">Accept</span></span>|<span data-ttu-id="207ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="207ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="207ef-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="207ef-127">Request body</span></span>
<span data-ttu-id="207ef-128">在请求正文中，提供 windowsPhone81TrustedRootCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="207ef-128">In the request body, supply a JSON representation for the windowsPhone81TrustedRootCertificate object.</span></span>

<span data-ttu-id="207ef-129">下表显示时创建 windowsPhone81TrustedRootCertificate 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="207ef-129">The following table shows the properties that are required when you create the windowsPhone81TrustedRootCertificate.</span></span>

|<span data-ttu-id="207ef-130">属性</span><span class="sxs-lookup"><span data-stu-id="207ef-130">Property</span></span>|<span data-ttu-id="207ef-131">类型</span><span class="sxs-lookup"><span data-stu-id="207ef-131">Type</span></span>|<span data-ttu-id="207ef-132">说明</span><span class="sxs-lookup"><span data-stu-id="207ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="207ef-133">id</span><span class="sxs-lookup"><span data-stu-id="207ef-133">id</span></span>|<span data-ttu-id="207ef-134">String</span><span class="sxs-lookup"><span data-stu-id="207ef-134">String</span></span>|<span data-ttu-id="207ef-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="207ef-135">Key of the entity.</span></span> <span data-ttu-id="207ef-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="207ef-137">lastModifiedDateTime</span></span>|<span data-ttu-id="207ef-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="207ef-138">DateTimeOffset</span></span>|<span data-ttu-id="207ef-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="207ef-139">DateTime the object was last modified.</span></span> <span data-ttu-id="207ef-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="207ef-141">roleScopeTagIds</span></span>|<span data-ttu-id="207ef-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="207ef-142">String collection</span></span>|<span data-ttu-id="207ef-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="207ef-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="207ef-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="207ef-145">supportsScopeTags</span></span>|<span data-ttu-id="207ef-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="207ef-146">Boolean</span></span>|<span data-ttu-id="207ef-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="207ef-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="207ef-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="207ef-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="207ef-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="207ef-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="207ef-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="207ef-150">This property is read-only.</span></span> <span data-ttu-id="207ef-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="207ef-152">createdDateTime</span></span>|<span data-ttu-id="207ef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="207ef-153">DateTimeOffset</span></span>|<span data-ttu-id="207ef-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="207ef-154">DateTime the object was created.</span></span> <span data-ttu-id="207ef-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-156">description</span><span class="sxs-lookup"><span data-stu-id="207ef-156">description</span></span>|<span data-ttu-id="207ef-157">String</span><span class="sxs-lookup"><span data-stu-id="207ef-157">String</span></span>|<span data-ttu-id="207ef-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="207ef-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="207ef-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-160">displayName</span><span class="sxs-lookup"><span data-stu-id="207ef-160">displayName</span></span>|<span data-ttu-id="207ef-161">String</span><span class="sxs-lookup"><span data-stu-id="207ef-161">String</span></span>|<span data-ttu-id="207ef-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="207ef-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="207ef-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-164">version</span><span class="sxs-lookup"><span data-stu-id="207ef-164">version</span></span>|<span data-ttu-id="207ef-165">Int32</span><span class="sxs-lookup"><span data-stu-id="207ef-165">Int32</span></span>|<span data-ttu-id="207ef-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="207ef-166">Version of the device configuration.</span></span> <span data-ttu-id="207ef-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="207ef-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="207ef-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="207ef-168">trustedRootCertificate</span></span>|<span data-ttu-id="207ef-169">Binary</span><span class="sxs-lookup"><span data-stu-id="207ef-169">Binary</span></span>|<span data-ttu-id="207ef-170">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="207ef-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="207ef-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="207ef-171">certFileName</span></span>|<span data-ttu-id="207ef-172">String</span><span class="sxs-lookup"><span data-stu-id="207ef-172">String</span></span>|<span data-ttu-id="207ef-173">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="207ef-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="207ef-174">响应</span><span class="sxs-lookup"><span data-stu-id="207ef-174">Response</span></span>
<span data-ttu-id="207ef-175">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="207ef-175">If successful, this method returns a `201 Created` response code and a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="207ef-176">示例</span><span class="sxs-lookup"><span data-stu-id="207ef-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="207ef-177">请求</span><span class="sxs-lookup"><span data-stu-id="207ef-177">Request</span></span>
<span data-ttu-id="207ef-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="207ef-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="207ef-179">响应</span><span class="sxs-lookup"><span data-stu-id="207ef-179">Response</span></span>
<span data-ttu-id="207ef-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="207ef-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.windowsPhone81TrustedRootCertificate",
  "id": "6316bf01-bf01-6316-01bf-166301bf1663",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value"
}
```




