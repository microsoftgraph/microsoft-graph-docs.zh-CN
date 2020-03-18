---
title: 更新 deviceManagementDerivedCredentialSettings
description: 更新 deviceManagementDerivedCredentialSettings 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 534b388975f40e269f006414a6dd39885211f7aa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800996"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="b6259-103">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="b6259-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="b6259-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6259-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6259-106">更新[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6259-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6259-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6259-107">Prerequisites</span></span>
<span data-ttu-id="b6259-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6259-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6259-110">Permission type</span></span>|<span data-ttu-id="b6259-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6259-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6259-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6259-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6259-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="b6259-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6259-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6259-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b6259-115">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="b6259-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="b6259-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6259-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6259-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6259-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6259-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6259-118">Not supported.</span></span>|
|<span data-ttu-id="b6259-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6259-119">Application</span></span>||
| <span data-ttu-id="b6259-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="b6259-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b6259-121">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6259-121">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b6259-122">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="b6259-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="b6259-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6259-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6259-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6259-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="b6259-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6259-125">Request headers</span></span>
|<span data-ttu-id="b6259-126">标头</span><span class="sxs-lookup"><span data-stu-id="b6259-126">Header</span></span>|<span data-ttu-id="b6259-127">值</span><span class="sxs-lookup"><span data-stu-id="b6259-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6259-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6259-128">Authorization</span></span>|<span data-ttu-id="b6259-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6259-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6259-130">接受</span><span class="sxs-lookup"><span data-stu-id="b6259-130">Accept</span></span>|<span data-ttu-id="b6259-131">application/json</span><span class="sxs-lookup"><span data-stu-id="b6259-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6259-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6259-132">Request body</span></span>
<span data-ttu-id="b6259-133">在请求正文中，提供[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6259-133">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="b6259-134">下表显示创建[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6259-134">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="b6259-135">属性</span><span class="sxs-lookup"><span data-stu-id="b6259-135">Property</span></span>|<span data-ttu-id="b6259-136">类型</span><span class="sxs-lookup"><span data-stu-id="b6259-136">Type</span></span>|<span data-ttu-id="b6259-137">说明</span><span class="sxs-lookup"><span data-stu-id="b6259-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6259-138">id</span><span class="sxs-lookup"><span data-stu-id="b6259-138">id</span></span>|<span data-ttu-id="b6259-139">String</span><span class="sxs-lookup"><span data-stu-id="b6259-139">String</span></span>|<span data-ttu-id="b6259-140">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b6259-140">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="b6259-141">**RA 策略**</span><span class="sxs-lookup"><span data-stu-id="b6259-141">**RA Policy**</span></span>|
|<span data-ttu-id="b6259-142">helpUrl</span><span class="sxs-lookup"><span data-stu-id="b6259-142">helpUrl</span></span>|<span data-ttu-id="b6259-143">String</span><span class="sxs-lookup"><span data-stu-id="b6259-143">String</span></span>|<span data-ttu-id="b6259-144">最终用户在使用公司门户检索派生凭据时将可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="b6259-144">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="b6259-145">displayName</span><span class="sxs-lookup"><span data-stu-id="b6259-145">displayName</span></span>|<span data-ttu-id="b6259-146">String</span><span class="sxs-lookup"><span data-stu-id="b6259-146">String</span></span>|<span data-ttu-id="b6259-147">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b6259-147">The display name for the profile.</span></span>|
|<span data-ttu-id="b6259-148">常用</span><span class="sxs-lookup"><span data-stu-id="b6259-148">issuer</span></span>|<span data-ttu-id="b6259-149">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="b6259-149">deviceManagementDerivedCredentialIssuer</span></span>|<span data-ttu-id="b6259-150">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="b6259-150">The derived credential provider to use.</span></span> <span data-ttu-id="b6259-151">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="b6259-151">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="b6259-152">notificationType</span><span class="sxs-lookup"><span data-stu-id="b6259-152">notificationType</span></span>|<span data-ttu-id="b6259-153">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="b6259-153">deviceManagementDerivedCredentialNotificationType</span></span>|<span data-ttu-id="b6259-154">用于通知最终用户打开公司门户以传递使用证书到设备的 Wi-fi、VPN 或电子邮件配置文件的方法。</span><span class="sxs-lookup"><span data-stu-id="b6259-154">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="b6259-155">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="b6259-155">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="b6259-156">响应</span><span class="sxs-lookup"><span data-stu-id="b6259-156">Response</span></span>
<span data-ttu-id="b6259-157">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6259-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6259-158">示例</span><span class="sxs-lookup"><span data-stu-id="b6259-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6259-159">请求</span><span class="sxs-lookup"><span data-stu-id="b6259-159">Request</span></span>
<span data-ttu-id="b6259-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6259-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="b6259-161">响应</span><span class="sxs-lookup"><span data-stu-id="b6259-161">Response</span></span>
<span data-ttu-id="b6259-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6259-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








