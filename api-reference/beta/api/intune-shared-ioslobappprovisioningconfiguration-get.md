---
title: 获取 iosLobAppProvisioningConfiguration
description: 读取 iosLobAppProvisioningConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 76646d93979c15604a9dce14a6e524903a958e80
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863161"
---
# <a name="get-ioslobappprovisioningconfiguration"></a><span data-ttu-id="5acb8-103">获取 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="5acb8-103">Get iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="5acb8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5acb8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5acb8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5acb8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5acb8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5acb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5acb8-107">读取 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5acb8-107">Read properties and relationships of the [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5acb8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5acb8-108">Prerequisites</span></span>
<span data-ttu-id="5acb8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5acb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5acb8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5acb8-111">Permission type</span></span>|<span data-ttu-id="5acb8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5acb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5acb8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5acb8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5acb8-114">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="5acb8-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="5acb8-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5acb8-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="5acb8-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="5acb8-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5acb8-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5acb8-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5acb8-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5acb8-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5acb8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5acb8-119">Not supported.</span></span>|
|<span data-ttu-id="5acb8-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5acb8-120">Application</span></span>||
| <span data-ttu-id="5acb8-121">&nbsp; &nbsp; **应用程序**</span><span class="sxs-lookup"><span data-stu-id="5acb8-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="5acb8-122">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5acb8-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="5acb8-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="5acb8-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="5acb8-124">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5acb8-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5acb8-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5acb8-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5acb8-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5acb8-126">Optional query parameters</span></span>
<span data-ttu-id="5acb8-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5acb8-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5acb8-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="5acb8-128">Request headers</span></span>
|<span data-ttu-id="5acb8-129">标头</span><span class="sxs-lookup"><span data-stu-id="5acb8-129">Header</span></span>|<span data-ttu-id="5acb8-130">值</span><span class="sxs-lookup"><span data-stu-id="5acb8-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5acb8-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="5acb8-131">Authorization</span></span>|<span data-ttu-id="5acb8-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5acb8-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5acb8-133">接受</span><span class="sxs-lookup"><span data-stu-id="5acb8-133">Accept</span></span>|<span data-ttu-id="5acb8-134">application/json</span><span class="sxs-lookup"><span data-stu-id="5acb8-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5acb8-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="5acb8-135">Request body</span></span>
<span data-ttu-id="5acb8-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5acb8-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5acb8-137">响应</span><span class="sxs-lookup"><span data-stu-id="5acb8-137">Response</span></span>
<span data-ttu-id="5acb8-138">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5acb8-138">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5acb8-139">示例</span><span class="sxs-lookup"><span data-stu-id="5acb8-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5acb8-140">请求</span><span class="sxs-lookup"><span data-stu-id="5acb8-140">Request</span></span>
<span data-ttu-id="5acb8-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5acb8-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5acb8-142">响应</span><span class="sxs-lookup"><span data-stu-id="5acb8-142">Response</span></span>
<span data-ttu-id="5acb8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5acb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
    "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "payloadFileName": "Payload File Name value",
    "payload": "cGF5bG9hZA==",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7
  }
}
```







