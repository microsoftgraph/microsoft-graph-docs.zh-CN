---
title: 更新 deviceManagementDerivedCredentialSettings
description: 更新 deviceManagementDerivedCredentialSettings 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 007126ea25822a635b946de00def06dbbf459c27
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36339748"
---
# <a name="update-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="a260a-103">更新 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="a260a-103">Update deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="a260a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a260a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a260a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a260a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a260a-106">更新[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a260a-106">Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a260a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a260a-107">Prerequisites</span></span>
<span data-ttu-id="a260a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a260a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a260a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a260a-110">Permission type</span></span>|<span data-ttu-id="a260a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a260a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a260a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a260a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a260a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a260a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a260a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a260a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a260a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a260a-115">Not supported.</span></span>|
|<span data-ttu-id="a260a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a260a-116">Application</span></span>|<span data-ttu-id="a260a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a260a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a260a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a260a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="request-headers"></a><span data-ttu-id="a260a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a260a-119">Request headers</span></span>
|<span data-ttu-id="a260a-120">标头</span><span class="sxs-lookup"><span data-stu-id="a260a-120">Header</span></span>|<span data-ttu-id="a260a-121">值</span><span class="sxs-lookup"><span data-stu-id="a260a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a260a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a260a-122">Authorization</span></span>|<span data-ttu-id="a260a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a260a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a260a-124">接受</span><span class="sxs-lookup"><span data-stu-id="a260a-124">Accept</span></span>|<span data-ttu-id="a260a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a260a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a260a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a260a-126">Request body</span></span>
<span data-ttu-id="a260a-127">在请求正文中, 提供[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a260a-127">In the request body, supply a JSON representation for the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object.</span></span>

<span data-ttu-id="a260a-128">下表显示创建[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a260a-128">The following table shows the properties that are required when you create the [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md).</span></span>

|<span data-ttu-id="a260a-129">属性</span><span class="sxs-lookup"><span data-stu-id="a260a-129">Property</span></span>|<span data-ttu-id="a260a-130">类型</span><span class="sxs-lookup"><span data-stu-id="a260a-130">Type</span></span>|<span data-ttu-id="a260a-131">说明</span><span class="sxs-lookup"><span data-stu-id="a260a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a260a-132">id</span><span class="sxs-lookup"><span data-stu-id="a260a-132">id</span></span>|<span data-ttu-id="a260a-133">String</span><span class="sxs-lookup"><span data-stu-id="a260a-133">String</span></span>|<span data-ttu-id="a260a-134">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="a260a-134">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="a260a-135">helpUrl</span><span class="sxs-lookup"><span data-stu-id="a260a-135">helpUrl</span></span>|<span data-ttu-id="a260a-136">String</span><span class="sxs-lookup"><span data-stu-id="a260a-136">String</span></span>|<span data-ttu-id="a260a-137">最终用户在使用公司门户检索派生凭据时将可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="a260a-137">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="a260a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a260a-138">displayName</span></span>|<span data-ttu-id="a260a-139">String</span><span class="sxs-lookup"><span data-stu-id="a260a-139">String</span></span>|<span data-ttu-id="a260a-140">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a260a-140">The display name for the profile.</span></span>|
|<span data-ttu-id="a260a-141">常用</span><span class="sxs-lookup"><span data-stu-id="a260a-141">issuer</span></span>|[<span data-ttu-id="a260a-142">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="a260a-142">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="a260a-143">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="a260a-143">The derived credential provider to use.</span></span> <span data-ttu-id="a260a-144">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="a260a-144">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="a260a-145">notificationType</span><span class="sxs-lookup"><span data-stu-id="a260a-145">notificationType</span></span>|[<span data-ttu-id="a260a-146">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="a260a-146">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-deviceconfig-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="a260a-147">用于通知最终用户打开公司门户以传递使用证书到设备的 Wi-fi、VPN 或电子邮件配置文件的方法。</span><span class="sxs-lookup"><span data-stu-id="a260a-147">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="a260a-148">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="a260a-148">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="a260a-149">响应</span><span class="sxs-lookup"><span data-stu-id="a260a-149">Response</span></span>
<span data-ttu-id="a260a-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a260a-150">If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a260a-151">示例</span><span class="sxs-lookup"><span data-stu-id="a260a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="a260a-152">请求</span><span class="sxs-lookup"><span data-stu-id="a260a-152">Request</span></span>
<span data-ttu-id="a260a-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a260a-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
Content-type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```

### <a name="response"></a><span data-ttu-id="a260a-154">响应</span><span class="sxs-lookup"><span data-stu-id="a260a-154">Response</span></span>
<span data-ttu-id="a260a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a260a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "bc650741-0741-bc65-4107-65bc410765bc",
  "helpUrl": "https://example.com/helpUrl/",
  "displayName": "Display Name value",
  "issuer": "entrustDatacard",
  "notificationType": "companyPortal"
}
```






