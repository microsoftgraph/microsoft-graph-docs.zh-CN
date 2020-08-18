---
title: 更新 deviceManagementDerivedCredentialSettings
description: 更新 deviceManagementDerivedCredentialSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c9a9e75da26ee8290c7890f59faec7c1f89ef24b
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792496"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="b1f90-103">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="b1f90-103">Update deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="b1f90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1f90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1f90-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1f90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1f90-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1f90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1f90-107">更新 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1f90-107">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1f90-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1f90-108">Prerequisites</span></span>
<span data-ttu-id="b1f90-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1f90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1f90-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1f90-111">Permission type</span></span>|<span data-ttu-id="b1f90-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1f90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1f90-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1f90-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b1f90-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="b1f90-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b1f90-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f90-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b1f90-116">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="b1f90-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="b1f90-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f90-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1f90-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1f90-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1f90-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1f90-119">Not supported.</span></span>|
|<span data-ttu-id="b1f90-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1f90-120">Application</span></span>||
| <span data-ttu-id="b1f90-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="b1f90-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b1f90-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f90-122">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b1f90-123">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="b1f90-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="b1f90-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1f90-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1f90-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1f90-125">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b1f90-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1f90-126">Request headers</span></span>
|<span data-ttu-id="b1f90-127">标头</span><span class="sxs-lookup"><span data-stu-id="b1f90-127">Header</span></span>|<span data-ttu-id="b1f90-128">值</span><span class="sxs-lookup"><span data-stu-id="b1f90-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1f90-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1f90-129">Authorization</span></span>|<span data-ttu-id="b1f90-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1f90-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1f90-131">接受</span><span class="sxs-lookup"><span data-stu-id="b1f90-131">Accept</span></span>|<span data-ttu-id="b1f90-132">application/json</span><span class="sxs-lookup"><span data-stu-id="b1f90-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1f90-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1f90-133">Request body</span></span>
<span data-ttu-id="b1f90-134">在请求正文中，提供 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1f90-134">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="b1f90-135">下表显示创建 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1f90-135">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="b1f90-136">属性</span><span class="sxs-lookup"><span data-stu-id="b1f90-136">Property</span></span>|<span data-ttu-id="b1f90-137">类型</span><span class="sxs-lookup"><span data-stu-id="b1f90-137">Type</span></span>|<span data-ttu-id="b1f90-138">说明</span><span class="sxs-lookup"><span data-stu-id="b1f90-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1f90-139">id</span><span class="sxs-lookup"><span data-stu-id="b1f90-139">id</span></span>|<span data-ttu-id="b1f90-140">String</span><span class="sxs-lookup"><span data-stu-id="b1f90-140">String</span></span>|<span data-ttu-id="b1f90-141">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="b1f90-141">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="b1f90-142">**RA 策略**</span><span class="sxs-lookup"><span data-stu-id="b1f90-142">**RA Policy**</span></span>|
|<span data-ttu-id="b1f90-143">helpUrl</span><span class="sxs-lookup"><span data-stu-id="b1f90-143">helpUrl</span></span>|<span data-ttu-id="b1f90-144">String</span><span class="sxs-lookup"><span data-stu-id="b1f90-144">String</span></span>|<span data-ttu-id="b1f90-145">最终用户在使用公司门户检索派生凭据时将可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="b1f90-145">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="b1f90-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b1f90-146">displayName</span></span>|<span data-ttu-id="b1f90-147">String</span><span class="sxs-lookup"><span data-stu-id="b1f90-147">String</span></span>|<span data-ttu-id="b1f90-148">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b1f90-148">The display name for the profile.</span></span>|
|<span data-ttu-id="b1f90-149">常用</span><span class="sxs-lookup"><span data-stu-id="b1f90-149">issuer</span></span>|[<span data-ttu-id="b1f90-150">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="b1f90-150">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-rapolicy-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="b1f90-151">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="b1f90-151">The derived credential provider to use.</span></span> <span data-ttu-id="b1f90-152">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="b1f90-152">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="b1f90-153">notificationType</span><span class="sxs-lookup"><span data-stu-id="b1f90-153">notificationType</span></span>|[<span data-ttu-id="b1f90-154">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="b1f90-154">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-rapolicy-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="b1f90-155">用于通知最终用户打开公司门户以传递使用证书到设备的 Wi-fi、VPN 或电子邮件配置文件的方法。</span><span class="sxs-lookup"><span data-stu-id="b1f90-155">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="b1f90-156">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="b1f90-156">Possible values are: `none`, `companyPortal`, `email`.</span></span>|


## <a name="response"></a><span data-ttu-id="b1f90-157">响应</span><span class="sxs-lookup"><span data-stu-id="b1f90-157">Response</span></span>
<span data-ttu-id="b1f90-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1f90-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1f90-159">示例</span><span class="sxs-lookup"><span data-stu-id="b1f90-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1f90-160">请求</span><span class="sxs-lookup"><span data-stu-id="b1f90-160">Request</span></span>
<span data-ttu-id="b1f90-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1f90-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 83

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings"
}
```

### <a name="response"></a><span data-ttu-id="b1f90-162">响应</span><span class="sxs-lookup"><span data-stu-id="b1f90-162">Response</span></span>
<span data-ttu-id="b1f90-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1f90-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 132

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc"
}
```







