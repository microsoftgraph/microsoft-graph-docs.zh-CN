---
title: 更新 windows81TrustedRootCertificate
description: 更新 windows81TrustedRootCertificate 对象的属性。
ms.openlocfilehash: c18c08e977d6fd034691836074e3f85b30e8f018
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043146"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="a5fa9-103">更新 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a5fa9-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="a5fa9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5fa9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5fa9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5fa9-107">更新[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-107">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5fa9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a5fa9-108">Prerequisites</span></span>
<span data-ttu-id="a5fa9-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a5fa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5fa9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5fa9-111">Permission type</span></span>|<span data-ttu-id="a5fa9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a5fa9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5fa9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5fa9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5fa9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fa9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5fa9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5fa9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5fa9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-116">Not supported.</span></span>|
|<span data-ttu-id="a5fa9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5fa9-117">Application</span></span>|<span data-ttu-id="a5fa9-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5fa9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5fa9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="a5fa9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5fa9-120">Request headers</span></span>
|<span data-ttu-id="a5fa9-121">标头</span><span class="sxs-lookup"><span data-stu-id="a5fa9-121">Header</span></span>|<span data-ttu-id="a5fa9-122">值</span><span class="sxs-lookup"><span data-stu-id="a5fa9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5fa9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5fa9-123">Authorization</span></span>|<span data-ttu-id="a5fa9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5fa9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5fa9-125">Accept</span></span>|<span data-ttu-id="a5fa9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5fa9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5fa9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5fa9-127">Request body</span></span>
<span data-ttu-id="a5fa9-128">在请求正文中，提供[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-128">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="a5fa9-129">下表显示时创建[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-129">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="a5fa9-130">属性</span><span class="sxs-lookup"><span data-stu-id="a5fa9-130">Property</span></span>|<span data-ttu-id="a5fa9-131">类型</span><span class="sxs-lookup"><span data-stu-id="a5fa9-131">Type</span></span>|<span data-ttu-id="a5fa9-132">说明</span><span class="sxs-lookup"><span data-stu-id="a5fa9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5fa9-133">id</span><span class="sxs-lookup"><span data-stu-id="a5fa9-133">id</span></span>|<span data-ttu-id="a5fa9-134">String</span><span class="sxs-lookup"><span data-stu-id="a5fa9-134">String</span></span>|<span data-ttu-id="a5fa9-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-135">Key of the entity.</span></span> <span data-ttu-id="a5fa9-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5fa9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a5fa9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5fa9-138">DateTimeOffset</span></span>|<span data-ttu-id="a5fa9-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a5fa9-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5fa9-141">roleScopeTagIds</span></span>|<span data-ttu-id="a5fa9-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="a5fa9-142">String collection</span></span>|<span data-ttu-id="a5fa9-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a5fa9-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a5fa9-145">supportsScopeTags</span></span>|<span data-ttu-id="a5fa9-146">布尔</span><span class="sxs-lookup"><span data-stu-id="a5fa9-146">Boolean</span></span>|<span data-ttu-id="a5fa9-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a5fa9-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a5fa9-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a5fa9-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-150">This property is read-only.</span></span> <span data-ttu-id="a5fa9-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5fa9-152">createdDateTime</span></span>|<span data-ttu-id="a5fa9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5fa9-153">DateTimeOffset</span></span>|<span data-ttu-id="a5fa9-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-154">DateTime the object was created.</span></span> <span data-ttu-id="a5fa9-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-156">description</span><span class="sxs-lookup"><span data-stu-id="a5fa9-156">description</span></span>|<span data-ttu-id="a5fa9-157">String</span><span class="sxs-lookup"><span data-stu-id="a5fa9-157">String</span></span>|<span data-ttu-id="a5fa9-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a5fa9-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a5fa9-160">displayName</span></span>|<span data-ttu-id="a5fa9-161">String</span><span class="sxs-lookup"><span data-stu-id="a5fa9-161">String</span></span>|<span data-ttu-id="a5fa9-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a5fa9-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-164">version</span><span class="sxs-lookup"><span data-stu-id="a5fa9-164">version</span></span>|<span data-ttu-id="a5fa9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a5fa9-165">Int32</span></span>|<span data-ttu-id="a5fa9-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-166">Version of the device configuration.</span></span> <span data-ttu-id="a5fa9-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a5fa9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a5fa9-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a5fa9-168">trustedRootCertificate</span></span>|<span data-ttu-id="a5fa9-169">二进制数</span><span class="sxs-lookup"><span data-stu-id="a5fa9-169">Binary</span></span>|<span data-ttu-id="a5fa9-170">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="a5fa9-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="a5fa9-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="a5fa9-171">certFileName</span></span>|<span data-ttu-id="a5fa9-172">字符串</span><span class="sxs-lookup"><span data-stu-id="a5fa9-172">String</span></span>|<span data-ttu-id="a5fa9-173">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-173">File name to display in UI.</span></span>|
|<span data-ttu-id="a5fa9-174">destinationStore</span><span class="sxs-lookup"><span data-stu-id="a5fa9-174">destinationStore</span></span>|[<span data-ttu-id="a5fa9-175">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="a5fa9-175">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="a5fa9-176">受信任根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-176">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="a5fa9-177">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-177">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="a5fa9-178">响应</span><span class="sxs-lookup"><span data-stu-id="a5fa9-178">Response</span></span>
<span data-ttu-id="a5fa9-179">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-179">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5fa9-180">示例</span><span class="sxs-lookup"><span data-stu-id="a5fa9-180">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5fa9-181">请求</span><span class="sxs-lookup"><span data-stu-id="a5fa9-181">Request</span></span>
<span data-ttu-id="a5fa9-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 419

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="a5fa9-183">响应</span><span class="sxs-lookup"><span data-stu-id="a5fa9-183">Response</span></span>
<span data-ttu-id="a5fa9-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a5fa9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 597

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
  "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```





