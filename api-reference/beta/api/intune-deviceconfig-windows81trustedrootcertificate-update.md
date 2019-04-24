---
title: 更新 windows81TrustedRootCertificate
description: 更新 windows81TrustedRootCertificate 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f8a60362ce178a9aa42c92e9c469b58577096c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515244"
---
# <a name="update-windows81trustedrootcertificate"></a><span data-ttu-id="6bdba-103">更新 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="6bdba-103">Update windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="6bdba-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6bdba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6bdba-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6bdba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6bdba-106">更新[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6bdba-106">Update the properties of a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6bdba-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6bdba-107">Prerequisites</span></span>
<span data-ttu-id="6bdba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6bdba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bdba-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6bdba-110">Permission type</span></span>|<span data-ttu-id="6bdba-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6bdba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bdba-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6bdba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6bdba-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bdba-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bdba-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6bdba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bdba-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bdba-115">Not supported.</span></span>|
|<span data-ttu-id="6bdba-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6bdba-116">Application</span></span>|<span data-ttu-id="6bdba-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6bdba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bdba-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6bdba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="6bdba-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6bdba-119">Request headers</span></span>
|<span data-ttu-id="6bdba-120">标头</span><span class="sxs-lookup"><span data-stu-id="6bdba-120">Header</span></span>|<span data-ttu-id="6bdba-121">值</span><span class="sxs-lookup"><span data-stu-id="6bdba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bdba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bdba-122">Authorization</span></span>|<span data-ttu-id="6bdba-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6bdba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bdba-124">接受</span><span class="sxs-lookup"><span data-stu-id="6bdba-124">Accept</span></span>|<span data-ttu-id="6bdba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6bdba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bdba-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6bdba-126">Request body</span></span>
<span data-ttu-id="6bdba-127">在请求正文中, 提供[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bdba-127">In the request body, supply a JSON representation for the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="6bdba-128">下表显示创建[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6bdba-128">The following table shows the properties that are required when you create the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="6bdba-129">属性</span><span class="sxs-lookup"><span data-stu-id="6bdba-129">Property</span></span>|<span data-ttu-id="6bdba-130">类型</span><span class="sxs-lookup"><span data-stu-id="6bdba-130">Type</span></span>|<span data-ttu-id="6bdba-131">说明</span><span class="sxs-lookup"><span data-stu-id="6bdba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bdba-132">id</span><span class="sxs-lookup"><span data-stu-id="6bdba-132">id</span></span>|<span data-ttu-id="6bdba-133">String</span><span class="sxs-lookup"><span data-stu-id="6bdba-133">String</span></span>|<span data-ttu-id="6bdba-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6bdba-134">Key of the entity.</span></span> <span data-ttu-id="6bdba-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdba-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6bdba-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bdba-137">DateTimeOffset</span></span>|<span data-ttu-id="6bdba-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6bdba-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6bdba-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6bdba-140">roleScopeTagIds</span></span>|<span data-ttu-id="6bdba-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6bdba-141">String collection</span></span>|<span data-ttu-id="6bdba-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6bdba-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6bdba-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6bdba-144">supportsScopeTags</span></span>|<span data-ttu-id="6bdba-145">布尔</span><span class="sxs-lookup"><span data-stu-id="6bdba-145">Boolean</span></span>|<span data-ttu-id="6bdba-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="6bdba-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6bdba-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="6bdba-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6bdba-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="6bdba-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6bdba-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="6bdba-149">This property is read-only.</span></span> <span data-ttu-id="6bdba-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bdba-151">createdDateTime</span></span>|<span data-ttu-id="6bdba-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bdba-152">DateTimeOffset</span></span>|<span data-ttu-id="6bdba-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6bdba-153">DateTime the object was created.</span></span> <span data-ttu-id="6bdba-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-155">description</span><span class="sxs-lookup"><span data-stu-id="6bdba-155">description</span></span>|<span data-ttu-id="6bdba-156">字符串</span><span class="sxs-lookup"><span data-stu-id="6bdba-156">String</span></span>|<span data-ttu-id="6bdba-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6bdba-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bdba-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6bdba-159">displayName</span></span>|<span data-ttu-id="6bdba-160">String</span><span class="sxs-lookup"><span data-stu-id="6bdba-160">String</span></span>|<span data-ttu-id="6bdba-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6bdba-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bdba-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-163">version</span><span class="sxs-lookup"><span data-stu-id="6bdba-163">version</span></span>|<span data-ttu-id="6bdba-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6bdba-164">Int32</span></span>|<span data-ttu-id="6bdba-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6bdba-165">Version of the device configuration.</span></span> <span data-ttu-id="6bdba-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6bdba-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bdba-167">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="6bdba-167">trustedRootCertificate</span></span>|<span data-ttu-id="6bdba-168">Binary</span><span class="sxs-lookup"><span data-stu-id="6bdba-168">Binary</span></span>|<span data-ttu-id="6bdba-169">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="6bdba-169">Trusted Root Certificate</span></span>|
|<span data-ttu-id="6bdba-170">certFileName</span><span class="sxs-lookup"><span data-stu-id="6bdba-170">certFileName</span></span>|<span data-ttu-id="6bdba-171">字符串</span><span class="sxs-lookup"><span data-stu-id="6bdba-171">String</span></span>|<span data-ttu-id="6bdba-172">要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="6bdba-172">File name to display in UI.</span></span>|
|<span data-ttu-id="6bdba-173">destinationStore</span><span class="sxs-lookup"><span data-stu-id="6bdba-173">destinationStore</span></span>|[<span data-ttu-id="6bdba-174">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="6bdba-174">certificateDestinationStore</span></span>](../resources/intune-deviceconfig-certificatedestinationstore.md)|<span data-ttu-id="6bdba-175">受信任的根证书的目标存储位置。</span><span class="sxs-lookup"><span data-stu-id="6bdba-175">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="6bdba-176">可取值为：`computerCertStoreRoot`、`computerCertStoreIntermediate`、`userCertStoreIntermediate`。</span><span class="sxs-lookup"><span data-stu-id="6bdba-176">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="6bdba-177">响应</span><span class="sxs-lookup"><span data-stu-id="6bdba-177">Response</span></span>
<span data-ttu-id="6bdba-178">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6bdba-178">If successful, this method returns a `200 OK` response code and an updated [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bdba-179">示例</span><span class="sxs-lookup"><span data-stu-id="6bdba-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bdba-180">请求</span><span class="sxs-lookup"><span data-stu-id="6bdba-180">Request</span></span>
<span data-ttu-id="6bdba-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6bdba-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
Content-type: application/json
Content-length: 425

{
  "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="6bdba-182">响应</span><span class="sxs-lookup"><span data-stu-id="6bdba-182">Response</span></span>
<span data-ttu-id="6bdba-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6bdba-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





