---
title: 创建 androidTrustedRootCertificate
description: 创建新的 androidTrustedRootCertificate 对象。
author: tfitzmac
ms.openlocfilehash: bd2272b71b562584f880b538d4b2fc412374dda8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354941"
---
# <a name="create-androidtrustedrootcertificate"></a><span data-ttu-id="01bf1-103">创建 androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="01bf1-103">Create androidTrustedRootCertificate</span></span>

> <span data-ttu-id="01bf1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01bf1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01bf1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01bf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01bf1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="01bf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01bf1-107">创建新的[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01bf1-107">Create a new [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01bf1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="01bf1-108">Prerequisites</span></span>
<span data-ttu-id="01bf1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="01bf1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01bf1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="01bf1-111">Permission type</span></span>|<span data-ttu-id="01bf1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="01bf1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01bf1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01bf1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01bf1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bf1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01bf1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01bf1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01bf1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="01bf1-116">Not supported.</span></span>|
|<span data-ttu-id="01bf1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="01bf1-117">Application</span></span>|<span data-ttu-id="01bf1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="01bf1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01bf1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01bf1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="01bf1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="01bf1-120">Request headers</span></span>
|<span data-ttu-id="01bf1-121">标头</span><span class="sxs-lookup"><span data-stu-id="01bf1-121">Header</span></span>|<span data-ttu-id="01bf1-122">值</span><span class="sxs-lookup"><span data-stu-id="01bf1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01bf1-123">授权</span><span class="sxs-lookup"><span data-stu-id="01bf1-123">Authorization</span></span>|<span data-ttu-id="01bf1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="01bf1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01bf1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="01bf1-125">Accept</span></span>|<span data-ttu-id="01bf1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="01bf1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01bf1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="01bf1-127">Request body</span></span>
<span data-ttu-id="01bf1-128">在请求正文中，提供 androidTrustedRootCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01bf1-128">In the request body, supply a JSON representation for the androidTrustedRootCertificate object.</span></span>

<span data-ttu-id="01bf1-129">下表显示时创建 androidTrustedRootCertificate 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="01bf1-129">The following table shows the properties that are required when you create the androidTrustedRootCertificate.</span></span>

|<span data-ttu-id="01bf1-130">属性</span><span class="sxs-lookup"><span data-stu-id="01bf1-130">Property</span></span>|<span data-ttu-id="01bf1-131">类型</span><span class="sxs-lookup"><span data-stu-id="01bf1-131">Type</span></span>|<span data-ttu-id="01bf1-132">说明</span><span class="sxs-lookup"><span data-stu-id="01bf1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01bf1-133">id</span><span class="sxs-lookup"><span data-stu-id="01bf1-133">id</span></span>|<span data-ttu-id="01bf1-134">String</span><span class="sxs-lookup"><span data-stu-id="01bf1-134">String</span></span>|<span data-ttu-id="01bf1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="01bf1-135">Key of the entity.</span></span> <span data-ttu-id="01bf1-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01bf1-137">lastModifiedDateTime</span></span>|<span data-ttu-id="01bf1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01bf1-138">DateTimeOffset</span></span>|<span data-ttu-id="01bf1-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01bf1-139">DateTime the object was last modified.</span></span> <span data-ttu-id="01bf1-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="01bf1-141">roleScopeTagIds</span></span>|<span data-ttu-id="01bf1-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="01bf1-142">String collection</span></span>|<span data-ttu-id="01bf1-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="01bf1-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="01bf1-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="01bf1-145">supportsScopeTags</span></span>|<span data-ttu-id="01bf1-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="01bf1-146">Boolean</span></span>|<span data-ttu-id="01bf1-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="01bf1-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="01bf1-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="01bf1-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="01bf1-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="01bf1-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="01bf1-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="01bf1-150">This property is read-only.</span></span> <span data-ttu-id="01bf1-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01bf1-152">createdDateTime</span></span>|<span data-ttu-id="01bf1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01bf1-153">DateTimeOffset</span></span>|<span data-ttu-id="01bf1-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="01bf1-154">DateTime the object was created.</span></span> <span data-ttu-id="01bf1-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-156">description</span><span class="sxs-lookup"><span data-stu-id="01bf1-156">description</span></span>|<span data-ttu-id="01bf1-157">String</span><span class="sxs-lookup"><span data-stu-id="01bf1-157">String</span></span>|<span data-ttu-id="01bf1-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="01bf1-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="01bf1-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-160">displayName</span><span class="sxs-lookup"><span data-stu-id="01bf1-160">displayName</span></span>|<span data-ttu-id="01bf1-161">String</span><span class="sxs-lookup"><span data-stu-id="01bf1-161">String</span></span>|<span data-ttu-id="01bf1-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="01bf1-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="01bf1-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-164">version</span><span class="sxs-lookup"><span data-stu-id="01bf1-164">version</span></span>|<span data-ttu-id="01bf1-165">Int32</span><span class="sxs-lookup"><span data-stu-id="01bf1-165">Int32</span></span>|<span data-ttu-id="01bf1-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="01bf1-166">Version of the device configuration.</span></span> <span data-ttu-id="01bf1-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="01bf1-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="01bf1-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="01bf1-168">trustedRootCertificate</span></span>|<span data-ttu-id="01bf1-169">Binary</span><span class="sxs-lookup"><span data-stu-id="01bf1-169">Binary</span></span>|<span data-ttu-id="01bf1-170">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="01bf1-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="01bf1-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="01bf1-171">certFileName</span></span>|<span data-ttu-id="01bf1-172">字符串</span><span class="sxs-lookup"><span data-stu-id="01bf1-172">String</span></span>|<span data-ttu-id="01bf1-173">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="01bf1-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="01bf1-174">响应</span><span class="sxs-lookup"><span data-stu-id="01bf1-174">Response</span></span>
<span data-ttu-id="01bf1-175">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="01bf1-175">If successful, this method returns a `201 Created` response code and a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01bf1-176">示例</span><span class="sxs-lookup"><span data-stu-id="01bf1-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="01bf1-177">请求</span><span class="sxs-lookup"><span data-stu-id="01bf1-177">Request</span></span>
<span data-ttu-id="01bf1-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01bf1-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 431

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="01bf1-179">响应</span><span class="sxs-lookup"><span data-stu-id="01bf1-179">Response</span></span>
<span data-ttu-id="01bf1-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01bf1-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
  "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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





