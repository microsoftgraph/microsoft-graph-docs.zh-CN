---
title: 创建 iosImportedPFXCertificateProfile
description: 创建新的 iosImportedPFXCertificateProfile 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52dd23a885ba8a036653a54bad1833a72b6ac3e0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30989160"
---
# <a name="create-iosimportedpfxcertificateprofile"></a><span data-ttu-id="606ee-103">创建 iosImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="606ee-103">Create iosImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="606ee-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="606ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="606ee-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="606ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="606ee-106">创建新的[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="606ee-106">Create a new [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="606ee-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="606ee-107">Prerequisites</span></span>
<span data-ttu-id="606ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="606ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="606ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="606ee-110">Permission type</span></span>|<span data-ttu-id="606ee-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="606ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="606ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="606ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="606ee-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="606ee-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="606ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="606ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="606ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="606ee-115">Not supported.</span></span>|
|<span data-ttu-id="606ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="606ee-116">Application</span></span>|<span data-ttu-id="606ee-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="606ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="606ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="606ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="606ee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="606ee-119">Request headers</span></span>
|<span data-ttu-id="606ee-120">标头</span><span class="sxs-lookup"><span data-stu-id="606ee-120">Header</span></span>|<span data-ttu-id="606ee-121">值</span><span class="sxs-lookup"><span data-stu-id="606ee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="606ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="606ee-122">Authorization</span></span>|<span data-ttu-id="606ee-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="606ee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="606ee-124">接受</span><span class="sxs-lookup"><span data-stu-id="606ee-124">Accept</span></span>|<span data-ttu-id="606ee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="606ee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="606ee-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="606ee-126">Request body</span></span>
<span data-ttu-id="606ee-127">在请求正文中, 提供 iosImportedPFXCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="606ee-127">In the request body, supply a JSON representation for the iosImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="606ee-128">下表显示创建 iosImportedPFXCertificateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="606ee-128">The following table shows the properties that are required when you create the iosImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="606ee-129">属性</span><span class="sxs-lookup"><span data-stu-id="606ee-129">Property</span></span>|<span data-ttu-id="606ee-130">类型</span><span class="sxs-lookup"><span data-stu-id="606ee-130">Type</span></span>|<span data-ttu-id="606ee-131">说明</span><span class="sxs-lookup"><span data-stu-id="606ee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="606ee-132">id</span><span class="sxs-lookup"><span data-stu-id="606ee-132">id</span></span>|<span data-ttu-id="606ee-133">String</span><span class="sxs-lookup"><span data-stu-id="606ee-133">String</span></span>|<span data-ttu-id="606ee-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="606ee-134">Key of the entity.</span></span> <span data-ttu-id="606ee-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="606ee-136">lastModifiedDateTime</span></span>|<span data-ttu-id="606ee-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="606ee-137">DateTimeOffset</span></span>|<span data-ttu-id="606ee-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="606ee-138">DateTime the object was last modified.</span></span> <span data-ttu-id="606ee-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="606ee-140">roleScopeTagIds</span></span>|<span data-ttu-id="606ee-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="606ee-141">String collection</span></span>|<span data-ttu-id="606ee-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="606ee-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="606ee-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="606ee-144">supportsScopeTags</span></span>|<span data-ttu-id="606ee-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="606ee-145">Boolean</span></span>|<span data-ttu-id="606ee-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="606ee-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="606ee-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="606ee-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="606ee-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="606ee-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="606ee-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="606ee-149">This property is read-only.</span></span> <span data-ttu-id="606ee-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="606ee-151">createdDateTime</span></span>|<span data-ttu-id="606ee-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="606ee-152">DateTimeOffset</span></span>|<span data-ttu-id="606ee-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="606ee-153">DateTime the object was created.</span></span> <span data-ttu-id="606ee-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-155">description</span><span class="sxs-lookup"><span data-stu-id="606ee-155">description</span></span>|<span data-ttu-id="606ee-156">String</span><span class="sxs-lookup"><span data-stu-id="606ee-156">String</span></span>|<span data-ttu-id="606ee-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="606ee-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="606ee-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-159">displayName</span><span class="sxs-lookup"><span data-stu-id="606ee-159">displayName</span></span>|<span data-ttu-id="606ee-160">String</span><span class="sxs-lookup"><span data-stu-id="606ee-160">String</span></span>|<span data-ttu-id="606ee-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="606ee-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="606ee-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-163">version</span><span class="sxs-lookup"><span data-stu-id="606ee-163">version</span></span>|<span data-ttu-id="606ee-164">Int32</span><span class="sxs-lookup"><span data-stu-id="606ee-164">Int32</span></span>|<span data-ttu-id="606ee-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="606ee-165">Version of the device configuration.</span></span> <span data-ttu-id="606ee-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="606ee-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="606ee-167">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="606ee-167">intendedPurpose</span></span>|[<span data-ttu-id="606ee-168">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="606ee-168">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="606ee-169">尚未记录。</span><span class="sxs-lookup"><span data-stu-id="606ee-169">Not yet documented.</span></span> <span data-ttu-id="606ee-170">可取值为：`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn` 或 `wifi`。</span><span class="sxs-lookup"><span data-stu-id="606ee-170">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="606ee-171">响应</span><span class="sxs-lookup"><span data-stu-id="606ee-171">Response</span></span>
<span data-ttu-id="606ee-172">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="606ee-172">If successful, this method returns a `201 Created` response code and a [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="606ee-173">示例</span><span class="sxs-lookup"><span data-stu-id="606ee-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="606ee-174">请求</span><span class="sxs-lookup"><span data-stu-id="606ee-174">Request</span></span>
<span data-ttu-id="606ee-175">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="606ee-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="606ee-176">响应</span><span class="sxs-lookup"><span data-stu-id="606ee-176">Response</span></span>
<span data-ttu-id="606ee-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="606ee-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
  "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "intendedPurpose": "smimeEncryption"
}
```




