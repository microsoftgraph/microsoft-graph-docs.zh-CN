---
title: 获取 deviceManagementDerivedCredentialSettings
description: 读取 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6b66790e7ff92c602dc29e57156920c647e11975
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537013"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="385a0-103">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="385a0-103">Get deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="385a0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="385a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="385a0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="385a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="385a0-106">读取[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="385a0-106">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="385a0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="385a0-107">Prerequisites</span></span>
<span data-ttu-id="385a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="385a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="385a0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="385a0-110">Permission type</span></span>|<span data-ttu-id="385a0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="385a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="385a0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="385a0-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="385a0-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="385a0-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="385a0-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="385a0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="385a0-115">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="385a0-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="385a0-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="385a0-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="385a0-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="385a0-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="385a0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="385a0-118">Not supported.</span></span>|
|<span data-ttu-id="385a0-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="385a0-119">Application</span></span>||
|<span data-ttu-id="385a0-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="385a0-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="385a0-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="385a0-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="385a0-122">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="385a0-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="385a0-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="385a0-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="385a0-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="385a0-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosVpnConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEasEmailProfileConfiguration/derivedCredentialSettings
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosDerivedCredentialAuthenticationConfiguration/derivedCredentialSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="385a0-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="385a0-125">Optional query parameters</span></span>
<span data-ttu-id="385a0-126">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="385a0-126">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="385a0-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="385a0-127">Request headers</span></span>
|<span data-ttu-id="385a0-128">标头</span><span class="sxs-lookup"><span data-stu-id="385a0-128">Header</span></span>|<span data-ttu-id="385a0-129">值</span><span class="sxs-lookup"><span data-stu-id="385a0-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="385a0-130">授权</span><span class="sxs-lookup"><span data-stu-id="385a0-130">Authorization</span></span>|<span data-ttu-id="385a0-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="385a0-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="385a0-132">接受</span><span class="sxs-lookup"><span data-stu-id="385a0-132">Accept</span></span>|<span data-ttu-id="385a0-133">application/json</span><span class="sxs-lookup"><span data-stu-id="385a0-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="385a0-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="385a0-134">Request body</span></span>
<span data-ttu-id="385a0-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="385a0-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="385a0-136">响应</span><span class="sxs-lookup"><span data-stu-id="385a0-136">Response</span></span>
<span data-ttu-id="385a0-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="385a0-137">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="385a0-138">示例</span><span class="sxs-lookup"><span data-stu-id="385a0-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="385a0-139">请求</span><span class="sxs-lookup"><span data-stu-id="385a0-139">Request</span></span>
<span data-ttu-id="385a0-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="385a0-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="385a0-141">响应</span><span class="sxs-lookup"><span data-stu-id="385a0-141">Response</span></span>
<span data-ttu-id="385a0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="385a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 155

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
    "id": "bc650741-0741-bc65-4107-65bc410765bc"
  }
}




