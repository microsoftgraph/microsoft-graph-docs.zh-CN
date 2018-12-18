---
title: 更新 windowsPhone81TrustedRootCertificate
description: 更新 windowsPhone81TrustedRootCertificate 对象的属性。
author: tfitzmac
ms.openlocfilehash: 052bf31f8e0c20231ca657ec5ebb99eb303f4fcc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327837"
---
# <a name="update-windowsphone81trustedrootcertificate"></a><span data-ttu-id="60729-103">更新 windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="60729-103">Update windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="60729-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="60729-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60729-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60729-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60729-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="60729-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60729-107">更新[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60729-107">Update the properties of a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="60729-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60729-108">Prerequisites</span></span>
<span data-ttu-id="60729-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="60729-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60729-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60729-111">Permission type</span></span>|<span data-ttu-id="60729-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60729-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60729-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60729-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60729-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60729-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60729-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60729-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60729-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60729-116">Not supported.</span></span>|
|<span data-ttu-id="60729-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60729-117">Application</span></span>|<span data-ttu-id="60729-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="60729-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60729-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60729-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="60729-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60729-120">Request headers</span></span>
|<span data-ttu-id="60729-121">标头</span><span class="sxs-lookup"><span data-stu-id="60729-121">Header</span></span>|<span data-ttu-id="60729-122">值</span><span class="sxs-lookup"><span data-stu-id="60729-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60729-123">授权</span><span class="sxs-lookup"><span data-stu-id="60729-123">Authorization</span></span>|<span data-ttu-id="60729-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60729-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60729-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60729-125">Accept</span></span>|<span data-ttu-id="60729-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60729-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60729-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60729-127">Request body</span></span>
<span data-ttu-id="60729-128">在请求正文中，提供[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60729-128">In the request body, supply a JSON representation for the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object.</span></span>

<span data-ttu-id="60729-129">下表显示时创建[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60729-129">The following table shows the properties that are required when you create the [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

|<span data-ttu-id="60729-130">属性</span><span class="sxs-lookup"><span data-stu-id="60729-130">Property</span></span>|<span data-ttu-id="60729-131">类型</span><span class="sxs-lookup"><span data-stu-id="60729-131">Type</span></span>|<span data-ttu-id="60729-132">说明</span><span class="sxs-lookup"><span data-stu-id="60729-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60729-133">id</span><span class="sxs-lookup"><span data-stu-id="60729-133">id</span></span>|<span data-ttu-id="60729-134">String</span><span class="sxs-lookup"><span data-stu-id="60729-134">String</span></span>|<span data-ttu-id="60729-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60729-135">Key of the entity.</span></span> <span data-ttu-id="60729-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60729-137">lastModifiedDateTime</span></span>|<span data-ttu-id="60729-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60729-138">DateTimeOffset</span></span>|<span data-ttu-id="60729-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="60729-139">DateTime the object was last modified.</span></span> <span data-ttu-id="60729-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="60729-141">roleScopeTagIds</span></span>|<span data-ttu-id="60729-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="60729-142">String collection</span></span>|<span data-ttu-id="60729-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="60729-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="60729-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="60729-145">supportsScopeTags</span></span>|<span data-ttu-id="60729-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="60729-146">Boolean</span></span>|<span data-ttu-id="60729-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="60729-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="60729-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="60729-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="60729-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="60729-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="60729-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="60729-150">This property is read-only.</span></span> <span data-ttu-id="60729-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="60729-152">createdDateTime</span></span>|<span data-ttu-id="60729-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60729-153">DateTimeOffset</span></span>|<span data-ttu-id="60729-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="60729-154">DateTime the object was created.</span></span> <span data-ttu-id="60729-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-156">description</span><span class="sxs-lookup"><span data-stu-id="60729-156">description</span></span>|<span data-ttu-id="60729-157">String</span><span class="sxs-lookup"><span data-stu-id="60729-157">String</span></span>|<span data-ttu-id="60729-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="60729-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="60729-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-160">displayName</span><span class="sxs-lookup"><span data-stu-id="60729-160">displayName</span></span>|<span data-ttu-id="60729-161">String</span><span class="sxs-lookup"><span data-stu-id="60729-161">String</span></span>|<span data-ttu-id="60729-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="60729-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="60729-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-164">version</span><span class="sxs-lookup"><span data-stu-id="60729-164">version</span></span>|<span data-ttu-id="60729-165">Int32</span><span class="sxs-lookup"><span data-stu-id="60729-165">Int32</span></span>|<span data-ttu-id="60729-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="60729-166">Version of the device configuration.</span></span> <span data-ttu-id="60729-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="60729-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="60729-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="60729-168">trustedRootCertificate</span></span>|<span data-ttu-id="60729-169">Binary</span><span class="sxs-lookup"><span data-stu-id="60729-169">Binary</span></span>|<span data-ttu-id="60729-170">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="60729-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="60729-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="60729-171">certFileName</span></span>|<span data-ttu-id="60729-172">字符串</span><span class="sxs-lookup"><span data-stu-id="60729-172">String</span></span>|<span data-ttu-id="60729-173">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="60729-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="60729-174">响应</span><span class="sxs-lookup"><span data-stu-id="60729-174">Response</span></span>
<span data-ttu-id="60729-175">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60729-175">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60729-176">示例</span><span class="sxs-lookup"><span data-stu-id="60729-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="60729-177">请求</span><span class="sxs-lookup"><span data-stu-id="60729-177">Request</span></span>
<span data-ttu-id="60729-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60729-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
Content-type: application/json
Content-length: 363

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
  "certFileName": "Cert File Name value"
}
```

### <a name="response"></a><span data-ttu-id="60729-179">响应</span><span class="sxs-lookup"><span data-stu-id="60729-179">Response</span></span>
<span data-ttu-id="60729-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60729-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





