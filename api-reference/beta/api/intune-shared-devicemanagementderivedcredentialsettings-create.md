---
title: 创建 deviceManagementDerivedCredentialSettings
description: 创建新的 deviceManagementDerivedCredentialSettings 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a605c0f868eab3deabbc854b27d62cc9e97769b1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37194577"
---
# <a name="create-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="cedfc-103">创建 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="cedfc-103">Create deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="cedfc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cedfc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cedfc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cedfc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cedfc-106">创建新的[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cedfc-106">Create a new [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cedfc-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cedfc-107">Prerequisites</span></span>
<span data-ttu-id="cedfc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cedfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cedfc-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cedfc-110">Permission type</span></span>|<span data-ttu-id="cedfc-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cedfc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cedfc-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cedfc-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="cedfc-113">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="cedfc-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="cedfc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cedfc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cedfc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cedfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cedfc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cedfc-116">Not supported.</span></span>|
|<span data-ttu-id="cedfc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cedfc-117">Application</span></span>||
|<span data-ttu-id="cedfc-118">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="cedfc-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="cedfc-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cedfc-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cedfc-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cedfc-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="cedfc-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cedfc-121">Request headers</span></span>
|<span data-ttu-id="cedfc-122">标头</span><span class="sxs-lookup"><span data-stu-id="cedfc-122">Header</span></span>|<span data-ttu-id="cedfc-123">值</span><span class="sxs-lookup"><span data-stu-id="cedfc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cedfc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cedfc-124">Authorization</span></span>|<span data-ttu-id="cedfc-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cedfc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cedfc-126">接受</span><span class="sxs-lookup"><span data-stu-id="cedfc-126">Accept</span></span>|<span data-ttu-id="cedfc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="cedfc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cedfc-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cedfc-128">Request body</span></span>
<span data-ttu-id="cedfc-129">在请求正文中，提供 deviceManagementDerivedCredentialSettings 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cedfc-129">In the request body, supply a JSON representation for the deviceManagementDerivedCredentialSettings object.</span></span>

<span data-ttu-id="cedfc-130">下表显示创建 deviceManagementDerivedCredentialSettings 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cedfc-130">The following table shows the properties that are required when you create the deviceManagementDerivedCredentialSettings.</span></span>

|<span data-ttu-id="cedfc-131">属性</span><span class="sxs-lookup"><span data-stu-id="cedfc-131">Property</span></span>|<span data-ttu-id="cedfc-132">类型</span><span class="sxs-lookup"><span data-stu-id="cedfc-132">Type</span></span>|<span data-ttu-id="cedfc-133">说明</span><span class="sxs-lookup"><span data-stu-id="cedfc-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cedfc-134">id</span><span class="sxs-lookup"><span data-stu-id="cedfc-134">id</span></span>|<span data-ttu-id="cedfc-135">String</span><span class="sxs-lookup"><span data-stu-id="cedfc-135">String</span></span>|<span data-ttu-id="cedfc-136">派生凭据的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="cedfc-136">Unique identifier for the Derived Credential</span></span>|
|<span data-ttu-id="cedfc-137">helpUrl</span><span class="sxs-lookup"><span data-stu-id="cedfc-137">helpUrl</span></span>|<span data-ttu-id="cedfc-138">String</span><span class="sxs-lookup"><span data-stu-id="cedfc-138">String</span></span>|<span data-ttu-id="cedfc-139">最终用户在使用公司门户检索派生凭据时将可访问的 URL。</span><span class="sxs-lookup"><span data-stu-id="cedfc-139">The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.</span></span>|
|<span data-ttu-id="cedfc-140">displayName</span><span class="sxs-lookup"><span data-stu-id="cedfc-140">displayName</span></span>|<span data-ttu-id="cedfc-141">String</span><span class="sxs-lookup"><span data-stu-id="cedfc-141">String</span></span>|<span data-ttu-id="cedfc-142">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cedfc-142">The display name for the profile.</span></span>|
|<span data-ttu-id="cedfc-143">常用</span><span class="sxs-lookup"><span data-stu-id="cedfc-143">issuer</span></span>|[<span data-ttu-id="cedfc-144">deviceManagementDerivedCredentialIssuer</span><span class="sxs-lookup"><span data-stu-id="cedfc-144">deviceManagementDerivedCredentialIssuer</span></span>](../resources/intune-shared-devicemanagementderivedcredentialissuer.md)|<span data-ttu-id="cedfc-145">要使用的派生凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="cedfc-145">The derived credential provider to use.</span></span> <span data-ttu-id="cedfc-146">可取值为：`intercede`、`entrustDatacard`、`purebred`。</span><span class="sxs-lookup"><span data-stu-id="cedfc-146">Possible values are: `intercede`, `entrustDatacard`, `purebred`.</span></span>|
|<span data-ttu-id="cedfc-147">notificationType</span><span class="sxs-lookup"><span data-stu-id="cedfc-147">notificationType</span></span>|[<span data-ttu-id="cedfc-148">deviceManagementDerivedCredentialNotificationType</span><span class="sxs-lookup"><span data-stu-id="cedfc-148">deviceManagementDerivedCredentialNotificationType</span></span>](../resources/intune-shared-devicemanagementderivedcredentialnotificationtype.md)|<span data-ttu-id="cedfc-149">用于通知最终用户打开公司门户以传递使用证书到设备的 Wi-fi、VPN 或电子邮件配置文件的方法。</span><span class="sxs-lookup"><span data-stu-id="cedfc-149">The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device.</span></span> <span data-ttu-id="cedfc-150">可取值为：`none`、`companyPortal`、`email`。</span><span class="sxs-lookup"><span data-stu-id="cedfc-150">Possible values are: `none`, `companyPortal`, `email`.</span></span>|



## <a name="response"></a><span data-ttu-id="cedfc-151">响应</span><span class="sxs-lookup"><span data-stu-id="cedfc-151">Response</span></span>
<span data-ttu-id="cedfc-152">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cedfc-152">If successful, this method returns a `201 Created` response code and a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cedfc-153">示例</span><span class="sxs-lookup"><span data-stu-id="cedfc-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="cedfc-154">请求</span><span class="sxs-lookup"><span data-stu-id="cedfc-154">Request</span></span>
<span data-ttu-id="cedfc-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cedfc-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
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

### <a name="response"></a><span data-ttu-id="cedfc-156">响应</span><span class="sxs-lookup"><span data-stu-id="cedfc-156">Response</span></span>
<span data-ttu-id="cedfc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cedfc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





