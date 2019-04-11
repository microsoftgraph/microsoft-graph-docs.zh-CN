---
title: 更新 windows10PFXImportCertificateProfile
description: 更新 windows10PFXImportCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77495930295654e04658f7908c3909a8c0c4863e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31800376"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="82477-103">更新 windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="82477-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="82477-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82477-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82477-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82477-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82477-106">更新[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82477-106">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82477-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="82477-107">Prerequisites</span></span>
<span data-ttu-id="82477-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82477-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82477-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="82477-110">Permission type</span></span>|<span data-ttu-id="82477-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82477-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82477-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82477-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82477-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82477-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82477-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82477-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82477-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="82477-115">Not supported.</span></span>|
|<span data-ttu-id="82477-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="82477-116">Application</span></span>|<span data-ttu-id="82477-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="82477-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82477-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82477-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82477-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="82477-119">Request headers</span></span>
|<span data-ttu-id="82477-120">标头</span><span class="sxs-lookup"><span data-stu-id="82477-120">Header</span></span>|<span data-ttu-id="82477-121">值</span><span class="sxs-lookup"><span data-stu-id="82477-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82477-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82477-122">Authorization</span></span>|<span data-ttu-id="82477-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82477-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82477-124">接受</span><span class="sxs-lookup"><span data-stu-id="82477-124">Accept</span></span>|<span data-ttu-id="82477-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82477-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82477-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="82477-126">Request body</span></span>
<span data-ttu-id="82477-127">在请求正文中, 提供[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82477-127">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="82477-128">下表显示创建[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82477-128">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="82477-129">属性</span><span class="sxs-lookup"><span data-stu-id="82477-129">Property</span></span>|<span data-ttu-id="82477-130">类型</span><span class="sxs-lookup"><span data-stu-id="82477-130">Type</span></span>|<span data-ttu-id="82477-131">说明</span><span class="sxs-lookup"><span data-stu-id="82477-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82477-132">id</span><span class="sxs-lookup"><span data-stu-id="82477-132">id</span></span>|<span data-ttu-id="82477-133">String</span><span class="sxs-lookup"><span data-stu-id="82477-133">String</span></span>|<span data-ttu-id="82477-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="82477-134">Key of the entity.</span></span> <span data-ttu-id="82477-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82477-136">lastModifiedDateTime</span></span>|<span data-ttu-id="82477-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82477-137">DateTimeOffset</span></span>|<span data-ttu-id="82477-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82477-138">DateTime the object was last modified.</span></span> <span data-ttu-id="82477-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82477-140">roleScopeTagIds</span></span>|<span data-ttu-id="82477-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="82477-141">String collection</span></span>|<span data-ttu-id="82477-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="82477-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82477-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="82477-144">supportsScopeTags</span></span>|<span data-ttu-id="82477-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="82477-145">Boolean</span></span>|<span data-ttu-id="82477-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="82477-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82477-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="82477-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82477-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="82477-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82477-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="82477-149">This property is read-only.</span></span> <span data-ttu-id="82477-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82477-151">createdDateTime</span></span>|<span data-ttu-id="82477-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82477-152">DateTimeOffset</span></span>|<span data-ttu-id="82477-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82477-153">DateTime the object was created.</span></span> <span data-ttu-id="82477-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-155">description</span><span class="sxs-lookup"><span data-stu-id="82477-155">description</span></span>|<span data-ttu-id="82477-156">String</span><span class="sxs-lookup"><span data-stu-id="82477-156">String</span></span>|<span data-ttu-id="82477-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="82477-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82477-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-159">displayName</span><span class="sxs-lookup"><span data-stu-id="82477-159">displayName</span></span>|<span data-ttu-id="82477-160">String</span><span class="sxs-lookup"><span data-stu-id="82477-160">String</span></span>|<span data-ttu-id="82477-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="82477-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82477-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-163">version</span><span class="sxs-lookup"><span data-stu-id="82477-163">version</span></span>|<span data-ttu-id="82477-164">Int32</span><span class="sxs-lookup"><span data-stu-id="82477-164">Int32</span></span>|<span data-ttu-id="82477-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="82477-165">Version of the device configuration.</span></span> <span data-ttu-id="82477-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82477-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82477-167">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="82477-167">keyStorageProvider</span></span>|[<span data-ttu-id="82477-168">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="82477-168">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="82477-169">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="82477-169">Not yet documented.</span></span> <span data-ttu-id="82477-170">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="82477-170">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="82477-171">响应</span><span class="sxs-lookup"><span data-stu-id="82477-171">Response</span></span>
<span data-ttu-id="82477-172">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="82477-172">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82477-173">示例</span><span class="sxs-lookup"><span data-stu-id="82477-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="82477-174">请求</span><span class="sxs-lookup"><span data-stu-id="82477-174">Request</span></span>
<span data-ttu-id="82477-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82477-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```

### <a name="response"></a><span data-ttu-id="82477-176">响应</span><span class="sxs-lookup"><span data-stu-id="82477-176">Response</span></span>
<span data-ttu-id="82477-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82477-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 489

{
  "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
  "id": "4244277a-277a-4244-7a27-44427a274442",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "keyStorageProvider": "useTpmKspOtherwiseFail"
}
```





