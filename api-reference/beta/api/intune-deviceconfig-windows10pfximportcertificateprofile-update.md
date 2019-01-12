---
title: 更新 windows10PFXImportCertificateProfile
description: 更新 windows10PFXImportCertificateProfile 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f055b39452097c398a9a41a860149cbcee969bb1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928624"
---
# <a name="update-windows10pfximportcertificateprofile"></a><span data-ttu-id="e02e7-103">更新 windows10PFXImportCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="e02e7-103">Update windows10PFXImportCertificateProfile</span></span>

> <span data-ttu-id="e02e7-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e02e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e02e7-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e02e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e02e7-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e02e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e02e7-107">更新[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e02e7-107">Update the properties of a [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e02e7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e02e7-108">Prerequisites</span></span>
<span data-ttu-id="e02e7-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e02e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e02e7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e02e7-111">Permission type</span></span>|<span data-ttu-id="e02e7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e02e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e02e7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e02e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e02e7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e02e7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e02e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e02e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e02e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e02e7-116">Not supported.</span></span>|
|<span data-ttu-id="e02e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e02e7-117">Application</span></span>|<span data-ttu-id="e02e7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e02e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e02e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e02e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e02e7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e02e7-120">Request headers</span></span>
|<span data-ttu-id="e02e7-121">标头</span><span class="sxs-lookup"><span data-stu-id="e02e7-121">Header</span></span>|<span data-ttu-id="e02e7-122">值</span><span class="sxs-lookup"><span data-stu-id="e02e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e02e7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e02e7-123">Authorization</span></span>|<span data-ttu-id="e02e7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e02e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e02e7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e02e7-125">Accept</span></span>|<span data-ttu-id="e02e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e02e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e02e7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e02e7-127">Request body</span></span>
<span data-ttu-id="e02e7-128">在请求正文中，提供[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e02e7-128">In the request body, supply a JSON representation for the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object.</span></span>

<span data-ttu-id="e02e7-129">下表显示时创建[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e02e7-129">The following table shows the properties that are required when you create the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md).</span></span>

|<span data-ttu-id="e02e7-130">属性</span><span class="sxs-lookup"><span data-stu-id="e02e7-130">Property</span></span>|<span data-ttu-id="e02e7-131">类型</span><span class="sxs-lookup"><span data-stu-id="e02e7-131">Type</span></span>|<span data-ttu-id="e02e7-132">说明</span><span class="sxs-lookup"><span data-stu-id="e02e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e02e7-133">id</span><span class="sxs-lookup"><span data-stu-id="e02e7-133">id</span></span>|<span data-ttu-id="e02e7-134">String</span><span class="sxs-lookup"><span data-stu-id="e02e7-134">String</span></span>|<span data-ttu-id="e02e7-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e02e7-135">Key of the entity.</span></span> <span data-ttu-id="e02e7-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e02e7-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e02e7-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e02e7-138">DateTimeOffset</span></span>|<span data-ttu-id="e02e7-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e02e7-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e02e7-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e02e7-141">roleScopeTagIds</span></span>|<span data-ttu-id="e02e7-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e02e7-142">String collection</span></span>|<span data-ttu-id="e02e7-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="e02e7-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e02e7-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e02e7-145">supportsScopeTags</span></span>|<span data-ttu-id="e02e7-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e02e7-146">Boolean</span></span>|<span data-ttu-id="e02e7-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="e02e7-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e02e7-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="e02e7-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e02e7-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="e02e7-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e02e7-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e02e7-150">This property is read-only.</span></span> <span data-ttu-id="e02e7-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e02e7-152">createdDateTime</span></span>|<span data-ttu-id="e02e7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e02e7-153">DateTimeOffset</span></span>|<span data-ttu-id="e02e7-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e02e7-154">DateTime the object was created.</span></span> <span data-ttu-id="e02e7-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-156">description</span><span class="sxs-lookup"><span data-stu-id="e02e7-156">description</span></span>|<span data-ttu-id="e02e7-157">String</span><span class="sxs-lookup"><span data-stu-id="e02e7-157">String</span></span>|<span data-ttu-id="e02e7-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e02e7-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e02e7-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-160">displayName</span><span class="sxs-lookup"><span data-stu-id="e02e7-160">displayName</span></span>|<span data-ttu-id="e02e7-161">String</span><span class="sxs-lookup"><span data-stu-id="e02e7-161">String</span></span>|<span data-ttu-id="e02e7-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e02e7-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e02e7-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-164">version</span><span class="sxs-lookup"><span data-stu-id="e02e7-164">version</span></span>|<span data-ttu-id="e02e7-165">Int32</span><span class="sxs-lookup"><span data-stu-id="e02e7-165">Int32</span></span>|<span data-ttu-id="e02e7-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e02e7-166">Version of the device configuration.</span></span> <span data-ttu-id="e02e7-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e02e7-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e02e7-168">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="e02e7-168">keyStorageProvider</span></span>|[<span data-ttu-id="e02e7-169">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="e02e7-169">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="e02e7-170">尚未编档。</span><span class="sxs-lookup"><span data-stu-id="e02e7-170">Not yet documented.</span></span> <span data-ttu-id="e02e7-171">可取值为：`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp`。</span><span class="sxs-lookup"><span data-stu-id="e02e7-171">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|



## <a name="response"></a><span data-ttu-id="e02e7-172">响应</span><span class="sxs-lookup"><span data-stu-id="e02e7-172">Response</span></span>
<span data-ttu-id="e02e7-173">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e02e7-173">If successful, this method returns a `200 OK` response code and an updated [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e02e7-174">示例</span><span class="sxs-lookup"><span data-stu-id="e02e7-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="e02e7-175">请求</span><span class="sxs-lookup"><span data-stu-id="e02e7-175">Request</span></span>
<span data-ttu-id="e02e7-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e02e7-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 306

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="e02e7-177">响应</span><span class="sxs-lookup"><span data-stu-id="e02e7-177">Response</span></span>
<span data-ttu-id="e02e7-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e02e7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





