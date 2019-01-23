---
title: 创建 windows10PFXImportCertificateProfile
description: 创建新的 windows10PFXImportCertificateProfile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93936f777c2cef72ecc4f770819ebeb42a11b832
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409242"
---
# <a name="create-windows10pfximportcertificateprofile"></a><span data-ttu-id="3fc2b-103">创建 windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="3fc2b-103">Create windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="3fc2b-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3fc2b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fc2b-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fc2b-107">创建新的[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-107">Create a new [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fc2b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3fc2b-108">Prerequisites</span></span>
<span data-ttu-id="3fc2b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3fc2b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3fc2b-111">Permission type</span></span>|<span data-ttu-id="3fc2b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3fc2b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fc2b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3fc2b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fc2b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fc2b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fc2b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3fc2b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fc2b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-116">Not supported.</span></span>|
|<span data-ttu-id="3fc2b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3fc2b-117">Application</span></span>|<span data-ttu-id="3fc2b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fc2b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3fc2b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3fc2b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3fc2b-120">Request headers</span></span>
|<span data-ttu-id="3fc2b-121">标头</span><span class="sxs-lookup"><span data-stu-id="3fc2b-121">Header</span></span>|<span data-ttu-id="3fc2b-122">值</span><span class="sxs-lookup"><span data-stu-id="3fc2b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fc2b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fc2b-123">Authorization</span></span>|<span data-ttu-id="3fc2b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fc2b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3fc2b-125">Accept</span></span>|<span data-ttu-id="3fc2b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fc2b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fc2b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3fc2b-127">Request body</span></span>
<span data-ttu-id="3fc2b-128">在请求正文中，提供 windows10PFXImportCertificateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-128">In the request body, supply a JSON representation for the windows10PFXImportCertificateProfile object.</span></span>

<span data-ttu-id="3fc2b-129">下表显示时创建 windows10PFXImportCertificateProfile 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-129">The following table shows the properties that are required when you create the windows10PFXImportCertificateProfile.</span></span>

|<span data-ttu-id="3fc2b-130">属性</span><span class="sxs-lookup"><span data-stu-id="3fc2b-130">Property</span></span>|<span data-ttu-id="3fc2b-131">类型</span><span class="sxs-lookup"><span data-stu-id="3fc2b-131">Type</span></span>|<span data-ttu-id="3fc2b-132">说明</span><span class="sxs-lookup"><span data-stu-id="3fc2b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fc2b-133">id</span><span class="sxs-lookup"><span data-stu-id="3fc2b-133">id</span></span>|<span data-ttu-id="3fc2b-134">String</span><span class="sxs-lookup"><span data-stu-id="3fc2b-134">String</span></span>|<span data-ttu-id="3fc2b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-135">Key of the entity.</span></span> <span data-ttu-id="3fc2b-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc2b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="3fc2b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc2b-138">DateTimeOffset</span></span>|<span data-ttu-id="3fc2b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="3fc2b-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3fc2b-141">roleScopeTagIds</span></span>|<span data-ttu-id="3fc2b-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="3fc2b-142">String collection</span></span>|<span data-ttu-id="3fc2b-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3fc2b-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3fc2b-145">supportsScopeTags</span></span>|<span data-ttu-id="3fc2b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fc2b-146">Boolean</span></span>|<span data-ttu-id="3fc2b-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3fc2b-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3fc2b-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3fc2b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-150">This property is read-only.</span></span> <span data-ttu-id="3fc2b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc2b-152">createdDateTime</span></span>|<span data-ttu-id="3fc2b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc2b-153">DateTimeOffset</span></span>|<span data-ttu-id="3fc2b-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-154">DateTime the object was created.</span></span> <span data-ttu-id="3fc2b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-156">description</span><span class="sxs-lookup"><span data-stu-id="3fc2b-156">description</span></span>|<span data-ttu-id="3fc2b-157">String</span><span class="sxs-lookup"><span data-stu-id="3fc2b-157">String</span></span>|<span data-ttu-id="3fc2b-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3fc2b-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="3fc2b-160">displayName</span></span>|<span data-ttu-id="3fc2b-161">String</span><span class="sxs-lookup"><span data-stu-id="3fc2b-161">String</span></span>|<span data-ttu-id="3fc2b-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3fc2b-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-164">version</span><span class="sxs-lookup"><span data-stu-id="3fc2b-164">version</span></span>|<span data-ttu-id="3fc2b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="3fc2b-165">Int32</span></span>|<span data-ttu-id="3fc2b-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-166">Version of the device configuration.</span></span> <span data-ttu-id="3fc2b-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3fc2b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fc2b-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="3fc2b-168">keyStorageProvider</span></span>|[<span data-ttu-id="3fc2b-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="3fc2b-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="3fc2b-170">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-170">Not yet documented.</span></span> <span data-ttu-id="3fc2b-171">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="3fc2b-172">响应</span><span class="sxs-lookup"><span data-stu-id="3fc2b-172">Response</span></span>
<span data-ttu-id="3fc2b-173">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-173">If successful, this method returns a `201 Created` response code and a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fc2b-174">示例</span><span class="sxs-lookup"><span data-stu-id="3fc2b-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fc2b-175">请求</span><span class="sxs-lookup"><span data-stu-id="3fc2b-175">Request</span></span>
<span data-ttu-id="3fc2b-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3fc2b-177">响应</span><span class="sxs-lookup"><span data-stu-id="3fc2b-177">Response</span></span>
<span data-ttu-id="3fc2b-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3fc2b-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




