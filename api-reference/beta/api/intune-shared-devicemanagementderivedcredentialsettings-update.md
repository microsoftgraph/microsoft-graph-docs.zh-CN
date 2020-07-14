---
title: 更新 deviceManagementDerivedCredentialSettings
description: 更新 deviceManagementDerivedCredentialSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf0460b25c3be317d9aebe7a91a02f7d2ae9f534
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123559"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="fc829-103">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="fc829-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="fc829-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc829-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc829-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc829-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc829-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc829-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc829-107">更新[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fc829-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc829-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc829-108">Prerequisites</span></span>
<span data-ttu-id="fc829-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fc829-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fc829-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc829-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc829-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc829-111">Permission type</span></span>|<span data-ttu-id="fc829-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc829-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc829-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc829-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fc829-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="fc829-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fc829-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc829-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="fc829-116">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="fc829-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="fc829-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc829-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc829-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc829-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc829-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc829-119">Not supported.</span></span>|
|<span data-ttu-id="fc829-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc829-120">Application</span></span>||
| <span data-ttu-id="fc829-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="fc829-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="fc829-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc829-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="fc829-123">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="fc829-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="fc829-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc829-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc829-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc829-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fc829-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc829-126">Request headers</span></span>
|<span data-ttu-id="fc829-127">标头</span><span class="sxs-lookup"><span data-stu-id="fc829-127">Header</span></span>|<span data-ttu-id="fc829-128">值</span><span class="sxs-lookup"><span data-stu-id="fc829-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc829-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc829-129">Authorization</span></span>|<span data-ttu-id="fc829-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc829-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc829-131">接受</span><span class="sxs-lookup"><span data-stu-id="fc829-131">Accept</span></span>|<span data-ttu-id="fc829-132">application/json</span><span class="sxs-lookup"><span data-stu-id="fc829-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc829-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc829-133">Request body</span></span>
<span data-ttu-id="fc829-134">在请求正文中，提供[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc829-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="fc829-135">下表显示创建[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc829-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="fc829-136">属性</span><span class="sxs-lookup"><span data-stu-id="fc829-136">Property</span></span>|<span data-ttu-id="fc829-137">类型</span><span class="sxs-lookup"><span data-stu-id="fc829-137">Type</span></span>|<span data-ttu-id="fc829-138">说明</span><span class="sxs-lookup"><span data-stu-id="fc829-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc829-139">id</span><span class="sxs-lookup"><span data-stu-id="fc829-139">id</span></span>|<span data-ttu-id="fc829-140">String</span><span class="sxs-lookup"><span data-stu-id="fc829-140">String</span></span>|<span data-ttu-id="fc829-141">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="fc829-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="fc829-142">**RA 策略**</span><span class="sxs-lookup"><span data-stu-id="fc829-142">**RA Policy**</span></span>|
|<span data-ttu-id="fc829-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="fc829-143">helpUrl</span></span>|<span data-ttu-id="fc829-144">String</span><span class="sxs-lookup"><span data-stu-id="fc829-144">String</span></span>|<span data-ttu-id="fc829-145">最终用户在使用公司门户检索派生凭据时将可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="fc829-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="fc829-146">displayName</span><span class="sxs-lookup"><span data-stu-id="fc829-146">displayName</span></span>|<span data-ttu-id="fc829-147">String</span><span class="sxs-lookup"><span data-stu-id="fc829-147">String</span></span>|<span data-ttu-id="fc829-148">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fc829-148">The display name for the profile.</span></span>|
|<span data-ttu-id="fc829-149">常用</span><span class="sxs-lookup"><span data-stu-id="fc829-149">issuer</span></span>|[<span data-ttu-id="fc829-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="fc829-150">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="fc829-151">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="fc829-151">The derived credential provider to use.</span></span> <span data-ttu-id="fc829-152">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="fc829-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="fc829-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="fc829-153">notificationType</span></span>|[<span data-ttu-id="fc829-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="fc829-154">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="fc829-155">用于通知最终用户打开公司门户以传递使用证书到设备的 Wi-fi、VPN 或电子邮件配置文件的方法。</span><span class="sxs-lookup"><span data-stu-id="fc829-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="fc829-156">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="fc829-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="fc829-157">响应</span><span class="sxs-lookup"><span data-stu-id="fc829-157">Response</span></span>
<span data-ttu-id="fc829-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc829-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc829-159">示例</span><span class="sxs-lookup"><span data-stu-id="fc829-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc829-160">请求</span><span class="sxs-lookup"><span data-stu-id="fc829-160">Request</span></span>
<span data-ttu-id="fc829-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc829-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="fc829-162">响应</span><span class="sxs-lookup"><span data-stu-id="fc829-162">Response</span></span>
<span data-ttu-id="fc829-163">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="fc829-163">Here is an example of the response.</span></span> <span data-ttu-id="fc829-164">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="fc829-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fc829-165">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fc829-165">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```







