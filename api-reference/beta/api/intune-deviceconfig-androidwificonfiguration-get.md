---
title: 获取 androidWiFiConfiguration
description: 读取 androidWiFiConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aadc8aa0e9c89d3959ea1eca10d6ef5deca6fe06
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166260"
---
# <a name="get-androidwificonfiguration"></a><span data-ttu-id="c7d31-103">获取 androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="c7d31-103">Get androidWiFiConfiguration</span></span>

> <span data-ttu-id="c7d31-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7d31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7d31-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7d31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7d31-106">读取[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7d31-106">Read properties and relationships of the [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7d31-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c7d31-107">Prerequisites</span></span>
<span data-ttu-id="c7d31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c7d31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7d31-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7d31-110">Permission type</span></span>|<span data-ttu-id="c7d31-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c7d31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7d31-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7d31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7d31-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7d31-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7d31-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7d31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7d31-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7d31-115">Not supported.</span></span>|
|<span data-ttu-id="c7d31-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7d31-116">Application</span></span>|<span data-ttu-id="c7d31-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c7d31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7d31-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7d31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7d31-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7d31-119">Optional query parameters</span></span>
<span data-ttu-id="c7d31-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7d31-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7d31-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7d31-121">Request headers</span></span>
|<span data-ttu-id="c7d31-122">标头</span><span class="sxs-lookup"><span data-stu-id="c7d31-122">Header</span></span>|<span data-ttu-id="c7d31-123">值</span><span class="sxs-lookup"><span data-stu-id="c7d31-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7d31-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7d31-124">Authorization</span></span>|<span data-ttu-id="c7d31-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c7d31-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7d31-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c7d31-126">Accept</span></span>|<span data-ttu-id="c7d31-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7d31-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7d31-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7d31-128">Request body</span></span>
<span data-ttu-id="c7d31-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7d31-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7d31-130">响应</span><span class="sxs-lookup"><span data-stu-id="c7d31-130">Response</span></span>
<span data-ttu-id="c7d31-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c7d31-131">If successful, this method returns a `200 OK` response code and [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7d31-132">示例</span><span class="sxs-lookup"><span data-stu-id="c7d31-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7d31-133">请求</span><span class="sxs-lookup"><span data-stu-id="c7d31-133">Request</span></span>
<span data-ttu-id="c7d31-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7d31-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c7d31-135">响应</span><span class="sxs-lookup"><span data-stu-id="c7d31-135">Response</span></span>
<span data-ttu-id="c7d31-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7d31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 658

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
    "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaEnterprise"
  }
}
```




