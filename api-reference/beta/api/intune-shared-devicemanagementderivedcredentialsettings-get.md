---
title: 获取 deviceManagementDerivedCredentialSettings
description: 读取 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fbbeb006243d5d59905ebca8246f0de05f0c247e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801010"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="79eec-103">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="79eec-103">Get deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="79eec-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="79eec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79eec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79eec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79eec-106">读取[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="79eec-106">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79eec-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="79eec-107">Prerequisites</span></span>
<span data-ttu-id="79eec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79eec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79eec-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79eec-110">Permission type</span></span>|<span data-ttu-id="79eec-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79eec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79eec-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79eec-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="79eec-113">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="79eec-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="79eec-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79eec-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79eec-115">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="79eec-115">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="79eec-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79eec-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79eec-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79eec-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79eec-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="79eec-118">Not supported.</span></span>|
|<span data-ttu-id="79eec-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="79eec-119">Application</span></span>||
|<span data-ttu-id="79eec-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="79eec-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="79eec-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79eec-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="79eec-122">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="79eec-122">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="79eec-123">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="79eec-123">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79eec-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79eec-124">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="79eec-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="79eec-125">Optional query parameters</span></span>
<span data-ttu-id="79eec-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="79eec-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79eec-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="79eec-127">Request headers</span></span>
|<span data-ttu-id="79eec-128">标头</span><span class="sxs-lookup"><span data-stu-id="79eec-128">Header</span></span>|<span data-ttu-id="79eec-129">值</span><span class="sxs-lookup"><span data-stu-id="79eec-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79eec-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="79eec-130">Authorization</span></span>|<span data-ttu-id="79eec-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79eec-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79eec-132">接受</span><span class="sxs-lookup"><span data-stu-id="79eec-132">Accept</span></span>|<span data-ttu-id="79eec-133">application/json</span><span class="sxs-lookup"><span data-stu-id="79eec-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79eec-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="79eec-134">Request body</span></span>
<span data-ttu-id="79eec-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79eec-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79eec-136">响应</span><span class="sxs-lookup"><span data-stu-id="79eec-136">Response</span></span>
<span data-ttu-id="79eec-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79eec-137">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79eec-138">示例</span><span class="sxs-lookup"><span data-stu-id="79eec-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="79eec-139">请求</span><span class="sxs-lookup"><span data-stu-id="79eec-139">Request</span></span>
<span data-ttu-id="79eec-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79eec-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="79eec-141">响应</span><span class="sxs-lookup"><span data-stu-id="79eec-141">Response</span></span>
<span data-ttu-id="79eec-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79eec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





