---
title: 创建 androidWorkProfileTrustedRootCertificate
description: 创建新的 androidWorkProfileTrustedRootCertificate 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fc819fb720d6620f03abd9cdb011cde8f71a86f5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424474"
---
# <a name="create-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="1a89d-103">创建 androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1a89d-103">Create androidWorkProfileTrustedRootCertificate</span></span>

> <span data-ttu-id="1a89d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1a89d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1a89d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1a89d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a89d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a89d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a89d-107">创建新的[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a89d-107">Create a new [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a89d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a89d-108">Prerequisites</span></span>
<span data-ttu-id="1a89d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1a89d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1a89d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a89d-111">Permission type</span></span>|<span data-ttu-id="1a89d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1a89d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a89d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a89d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a89d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a89d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1a89d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a89d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a89d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a89d-116">Not supported.</span></span>|
|<span data-ttu-id="1a89d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a89d-117">Application</span></span>|<span data-ttu-id="1a89d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a89d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a89d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a89d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1a89d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a89d-120">Request headers</span></span>
|<span data-ttu-id="1a89d-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a89d-121">Header</span></span>|<span data-ttu-id="1a89d-122">值</span><span class="sxs-lookup"><span data-stu-id="1a89d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a89d-123">授权</span><span class="sxs-lookup"><span data-stu-id="1a89d-123">Authorization</span></span>|<span data-ttu-id="1a89d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a89d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a89d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1a89d-125">Accept</span></span>|<span data-ttu-id="1a89d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a89d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a89d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a89d-127">Request body</span></span>
<span data-ttu-id="1a89d-128">在请求正文中，提供 androidWorkProfileTrustedRootCertificate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a89d-128">In the request body, supply a JSON representation for the androidWorkProfileTrustedRootCertificate object.</span></span>

<span data-ttu-id="1a89d-129">下表显示时创建 androidWorkProfileTrustedRootCertificate 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a89d-129">The following table shows the properties that are required when you create the androidWorkProfileTrustedRootCertificate.</span></span>

|<span data-ttu-id="1a89d-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a89d-130">Property</span></span>|<span data-ttu-id="1a89d-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a89d-131">Type</span></span>|<span data-ttu-id="1a89d-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a89d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a89d-133">id</span><span class="sxs-lookup"><span data-stu-id="1a89d-133">id</span></span>|<span data-ttu-id="1a89d-134">String</span><span class="sxs-lookup"><span data-stu-id="1a89d-134">String</span></span>|<span data-ttu-id="1a89d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a89d-135">Key of the entity.</span></span> <span data-ttu-id="1a89d-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a89d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1a89d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a89d-138">DateTimeOffset</span></span>|<span data-ttu-id="1a89d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a89d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1a89d-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a89d-141">roleScopeTagIds</span></span>|<span data-ttu-id="1a89d-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="1a89d-142">String collection</span></span>|<span data-ttu-id="1a89d-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="1a89d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a89d-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a89d-145">supportsScopeTags</span></span>|<span data-ttu-id="1a89d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a89d-146">Boolean</span></span>|<span data-ttu-id="1a89d-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="1a89d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a89d-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="1a89d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a89d-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="1a89d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a89d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1a89d-150">This property is read-only.</span></span> <span data-ttu-id="1a89d-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a89d-152">createdDateTime</span></span>|<span data-ttu-id="1a89d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a89d-153">DateTimeOffset</span></span>|<span data-ttu-id="1a89d-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1a89d-154">DateTime the object was created.</span></span> <span data-ttu-id="1a89d-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-156">description</span><span class="sxs-lookup"><span data-stu-id="1a89d-156">description</span></span>|<span data-ttu-id="1a89d-157">String</span><span class="sxs-lookup"><span data-stu-id="1a89d-157">String</span></span>|<span data-ttu-id="1a89d-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1a89d-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a89d-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1a89d-160">displayName</span></span>|<span data-ttu-id="1a89d-161">String</span><span class="sxs-lookup"><span data-stu-id="1a89d-161">String</span></span>|<span data-ttu-id="1a89d-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1a89d-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a89d-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-164">version</span><span class="sxs-lookup"><span data-stu-id="1a89d-164">version</span></span>|<span data-ttu-id="1a89d-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1a89d-165">Int32</span></span>|<span data-ttu-id="1a89d-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1a89d-166">Version of the device configuration.</span></span> <span data-ttu-id="1a89d-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a89d-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a89d-168">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="1a89d-168">trustedRootCertificate</span></span>|<span data-ttu-id="1a89d-169">Binary</span><span class="sxs-lookup"><span data-stu-id="1a89d-169">Binary</span></span>|<span data-ttu-id="1a89d-170">受信任的根证书</span><span class="sxs-lookup"><span data-stu-id="1a89d-170">Trusted Root Certificate</span></span>|
|<span data-ttu-id="1a89d-171">certFileName</span><span class="sxs-lookup"><span data-stu-id="1a89d-171">certFileName</span></span>|<span data-ttu-id="1a89d-172">String</span><span class="sxs-lookup"><span data-stu-id="1a89d-172">String</span></span>|<span data-ttu-id="1a89d-173">若要在 UI 中显示的文件名。</span><span class="sxs-lookup"><span data-stu-id="1a89d-173">File name to display in UI.</span></span>|



## <a name="response"></a><span data-ttu-id="1a89d-174">响应</span><span class="sxs-lookup"><span data-stu-id="1a89d-174">Response</span></span>
<span data-ttu-id="1a89d-175">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1a89d-175">If successful, this method returns a `201 Created` response code and a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a89d-176">示例</span><span class="sxs-lookup"><span data-stu-id="1a89d-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a89d-177">请求</span><span class="sxs-lookup"><span data-stu-id="1a89d-177">Request</span></span>
<span data-ttu-id="1a89d-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a89d-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
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

### <a name="response"></a><span data-ttu-id="1a89d-179">响应</span><span class="sxs-lookup"><span data-stu-id="1a89d-179">Response</span></span>
<span data-ttu-id="1a89d-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a89d-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 550

{
  "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
  "id": "37cc7454-7454-37cc-5474-cc375474cc37",
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




