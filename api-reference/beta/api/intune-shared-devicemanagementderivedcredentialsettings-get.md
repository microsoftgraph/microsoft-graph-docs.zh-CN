---
title: 获取 deviceManagementDerivedCredentialSettings
description: 读取 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7dda9173205802f18fa73063954aa133bb93ef9b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074424"
---
# <a name="get-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="41d06-103">获取 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="41d06-103">Get deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="41d06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41d06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41d06-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="41d06-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41d06-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41d06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41d06-107">读取 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="41d06-107">Read properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41d06-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41d06-108">Prerequisites</span></span>
<span data-ttu-id="41d06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d06-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41d06-111">Permission type</span></span>|<span data-ttu-id="41d06-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41d06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d06-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41d06-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="41d06-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="41d06-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="41d06-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d06-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41d06-116">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="41d06-116">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="41d06-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d06-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41d06-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41d06-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d06-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="41d06-119">Not supported.</span></span>|
|<span data-ttu-id="41d06-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="41d06-120">Application</span></span>||
|<span data-ttu-id="41d06-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="41d06-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="41d06-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d06-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41d06-123">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="41d06-123">&nbsp; &nbsp; **Resource Access Policy**</span></span> | <span data-ttu-id="41d06-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41d06-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d06-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41d06-125">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="41d06-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41d06-126">Optional query parameters</span></span>
<span data-ttu-id="41d06-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41d06-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41d06-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="41d06-128">Request headers</span></span>
|<span data-ttu-id="41d06-129">标头</span><span class="sxs-lookup"><span data-stu-id="41d06-129">Header</span></span>|<span data-ttu-id="41d06-130">值</span><span class="sxs-lookup"><span data-stu-id="41d06-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d06-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="41d06-131">Authorization</span></span>|<span data-ttu-id="41d06-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41d06-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d06-133">接受</span><span class="sxs-lookup"><span data-stu-id="41d06-133">Accept</span></span>|<span data-ttu-id="41d06-134">application/json</span><span class="sxs-lookup"><span data-stu-id="41d06-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d06-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="41d06-135">Request body</span></span>
<span data-ttu-id="41d06-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41d06-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41d06-137">响应</span><span class="sxs-lookup"><span data-stu-id="41d06-137">Response</span></span>
<span data-ttu-id="41d06-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41d06-138">If successful, this method returns a `200 OK` response code and [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d06-139">示例</span><span class="sxs-lookup"><span data-stu-id="41d06-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="41d06-140">请求</span><span class="sxs-lookup"><span data-stu-id="41d06-140">Request</span></span>
<span data-ttu-id="41d06-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41d06-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/derivedCredentialSettings
```

### <a name="response"></a><span data-ttu-id="41d06-142">响应</span><span class="sxs-lookup"><span data-stu-id="41d06-142">Response</span></span>
<span data-ttu-id="41d06-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41d06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







