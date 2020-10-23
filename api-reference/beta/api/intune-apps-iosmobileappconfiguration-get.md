---
title: 获取 iosMobileAppConfiguration
description: 读取 iosMobileAppConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 52ca4947c28a839b9c4a10acbf48ebac3ad09afe
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700302"
---
# <a name="get-iosmobileappconfiguration"></a><span data-ttu-id="b7c1b-103">获取 iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7c1b-103">Get iosMobileAppConfiguration</span></span>

<span data-ttu-id="b7c1b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7c1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7c1b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7c1b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c1b-107">读取 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-107">Read properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7c1b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7c1b-108">Prerequisites</span></span>
<span data-ttu-id="b7c1b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c1b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7c1b-111">Permission type</span></span>|<span data-ttu-id="b7c1b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7c1b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7c1b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7c1b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7c1b-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7c1b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b7c1b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7c1b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7c1b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-116">Not supported.</span></span>|
|<span data-ttu-id="b7c1b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7c1b-117">Application</span></span>|<span data-ttu-id="b7c1b-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7c1b-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7c1b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7c1b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7c1b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b7c1b-120">Optional query parameters</span></span>
<span data-ttu-id="b7c1b-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7c1b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7c1b-122">Request headers</span></span>
|<span data-ttu-id="b7c1b-123">标头</span><span class="sxs-lookup"><span data-stu-id="b7c1b-123">Header</span></span>|<span data-ttu-id="b7c1b-124">值</span><span class="sxs-lookup"><span data-stu-id="b7c1b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7c1b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c1b-125">Authorization</span></span>|<span data-ttu-id="b7c1b-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7c1b-127">接受</span><span class="sxs-lookup"><span data-stu-id="b7c1b-127">Accept</span></span>|<span data-ttu-id="b7c1b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b7c1b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c1b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7c1b-129">Request body</span></span>
<span data-ttu-id="b7c1b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7c1b-131">响应</span><span class="sxs-lookup"><span data-stu-id="b7c1b-131">Response</span></span>
<span data-ttu-id="b7c1b-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-132">If successful, this method returns a `200 OK` response code and [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c1b-133">示例</span><span class="sxs-lookup"><span data-stu-id="b7c1b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7c1b-134">请求</span><span class="sxs-lookup"><span data-stu-id="b7c1b-134">Request</span></span>
<span data-ttu-id="b7c1b-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b7c1b-136">响应</span><span class="sxs-lookup"><span data-stu-id="b7c1b-136">Response</span></span>
<span data-ttu-id="b7c1b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7c1b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 831

{
  "value": {
    "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
    "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
    "targetedMobileApps": [
      "Targeted Mobile Apps value"
    ],
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
    "settings": [
      {
        "@odata.type": "microsoft.graph.appConfigurationSettingItem",
        "appConfigKey": "App Config Key value",
        "appConfigKeyType": "integerType",
        "appConfigKeyValue": "App Config Key Value value"
      }
    ]
  }
}
```





