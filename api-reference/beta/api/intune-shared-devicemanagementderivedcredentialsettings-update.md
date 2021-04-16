---
title: 更新 deviceManagementDerivedCredentialSettings
description: 更新 deviceManagementDerivedCredentialSettings 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f94ac3eb5328cd8723008a25fd72e30347a1ac9
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867852"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="8040c-103">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="8040c-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="8040c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8040c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8040c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8040c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8040c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8040c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8040c-107">更新 [deviceManagementDerivedCredentialSettings 对象](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="8040c-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8040c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8040c-108">Prerequisites</span></span>
<span data-ttu-id="8040c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8040c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8040c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8040c-111">Permission type</span></span>|<span data-ttu-id="8040c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8040c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8040c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8040c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8040c-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8040c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8040c-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8040c-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8040c-116">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="8040c-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="8040c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8040c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8040c-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8040c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8040c-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="8040c-119">Not supported.</span></span>|
|<span data-ttu-id="8040c-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="8040c-120">Application</span></span>||
| <span data-ttu-id="8040c-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="8040c-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="8040c-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8040c-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="8040c-123">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="8040c-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="8040c-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8040c-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8040c-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8040c-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8040c-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="8040c-126">Request headers</span></span>
|<span data-ttu-id="8040c-127">标头</span><span class="sxs-lookup"><span data-stu-id="8040c-127">Header</span></span>|<span data-ttu-id="8040c-128">值</span><span class="sxs-lookup"><span data-stu-id="8040c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8040c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="8040c-129">Authorization</span></span>|<span data-ttu-id="8040c-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8040c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8040c-131">接受</span><span class="sxs-lookup"><span data-stu-id="8040c-131">Accept</span></span>|<span data-ttu-id="8040c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="8040c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8040c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="8040c-133">Request body</span></span>
<span data-ttu-id="8040c-134">在请求正文中，提供 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8040c-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="8040c-135">下表显示创建 [deviceManagementDerivedCredentialSettings 时所需的属性](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="8040c-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="8040c-136">属性</span><span class="sxs-lookup"><span data-stu-id="8040c-136">Property</span></span>|<span data-ttu-id="8040c-137">类型</span><span class="sxs-lookup"><span data-stu-id="8040c-137">Type</span></span>|<span data-ttu-id="8040c-138">说明</span><span class="sxs-lookup"><span data-stu-id="8040c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8040c-139">id</span><span class="sxs-lookup"><span data-stu-id="8040c-139">id</span></span>|<span data-ttu-id="8040c-140">String</span><span class="sxs-lookup"><span data-stu-id="8040c-140">String</span></span>|<span data-ttu-id="8040c-141">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="8040c-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="8040c-142">**RA 策略**</span><span class="sxs-lookup"><span data-stu-id="8040c-142">**RA Policy**</span></span>|
|<span data-ttu-id="8040c-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="8040c-143">helpUrl</span></span>|<span data-ttu-id="8040c-144">String</span><span class="sxs-lookup"><span data-stu-id="8040c-144">String</span></span>|<span data-ttu-id="8040c-145">最终用户在使用公司门户检索派生凭据时可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="8040c-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="8040c-146">displayName</span><span class="sxs-lookup"><span data-stu-id="8040c-146">displayName</span></span>|<span data-ttu-id="8040c-147">String</span><span class="sxs-lookup"><span data-stu-id="8040c-147">String</span></span>|<span data-ttu-id="8040c-148">配置文件显示名称的配置文件。</span><span class="sxs-lookup"><span data-stu-id="8040c-148">The display name for the profile.</span></span>|
|<span data-ttu-id="8040c-149">issuer</span><span class="sxs-lookup"><span data-stu-id="8040c-149">issuer</span></span>|[<span data-ttu-id="8040c-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="8040c-150">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-rapolicy-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="8040c-151">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="8040c-151">The derived credential provider to use.</span></span> <span data-ttu-id="8040c-152">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="8040c-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="8040c-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="8040c-153">notificationType</span></span>|[<span data-ttu-id="8040c-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="8040c-154">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-rapolicy-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="8040c-155">用于通知最终用户打开公司门户以将使用证书的 WLAN、VPN 或电子邮件配置文件发送到设备的方法。</span><span class="sxs-lookup"><span data-stu-id="8040c-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="8040c-156">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="8040c-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="8040c-157">响应</span><span class="sxs-lookup"><span data-stu-id="8040c-157">Response</span></span>
<span data-ttu-id="8040c-158">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8040c-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8040c-159">示例</span><span class="sxs-lookup"><span data-stu-id="8040c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="8040c-160">请求</span><span class="sxs-lookup"><span data-stu-id="8040c-160">Request</span></span>
<span data-ttu-id="8040c-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8040c-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="8040c-162">响应</span><span class="sxs-lookup"><span data-stu-id="8040c-162">Response</span></span>
<span data-ttu-id="8040c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8040c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```








