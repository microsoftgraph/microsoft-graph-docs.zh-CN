---
title: 获取 windows10TeamGeneralConfiguration
description: 读取 windows10TeamGeneralConfiguration 对象的属性和关系。
ms.openlocfilehash: 8e4a4cfcea1996835196fd42911a868022858d86
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010772"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="f8ec0-103">获取 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8ec0-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="f8ec0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8ec0-105">读取 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-105">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8ec0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8ec0-106">Prerequisites</span></span>
<span data-ttu-id="f8ec0-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f8ec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8ec0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8ec0-109">Permission type</span></span>|<span data-ttu-id="f8ec0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8ec0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8ec0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8ec0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f8ec0-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f8ec0-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f8ec0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8ec0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8ec0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-114">Not supported.</span></span>|
|<span data-ttu-id="f8ec0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8ec0-115">Application</span></span>|<span data-ttu-id="f8ec0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8ec0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8ec0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8ec0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8ec0-118">Optional query parameters</span></span>
<span data-ttu-id="f8ec0-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8ec0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8ec0-120">Request headers</span></span>
|<span data-ttu-id="f8ec0-121">标头</span><span class="sxs-lookup"><span data-stu-id="f8ec0-121">Header</span></span>|<span data-ttu-id="f8ec0-122">值</span><span class="sxs-lookup"><span data-stu-id="f8ec0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8ec0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8ec0-123">Authorization</span></span>|<span data-ttu-id="f8ec0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8ec0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8ec0-125">Accept</span></span>|<span data-ttu-id="f8ec0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8ec0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8ec0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8ec0-127">Request body</span></span>
<span data-ttu-id="f8ec0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8ec0-129">响应</span><span class="sxs-lookup"><span data-stu-id="f8ec0-129">Response</span></span>
<span data-ttu-id="f8ec0-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-130">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8ec0-131">示例</span><span class="sxs-lookup"><span data-stu-id="f8ec0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8ec0-132">请求</span><span class="sxs-lookup"><span data-stu-id="f8ec0-132">Request</span></span>
<span data-ttu-id="f8ec0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f8ec0-134">响应</span><span class="sxs-lookup"><span data-stu-id="f8ec0-134">Response</span></span>
<span data-ttu-id="f8ec0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8ec0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1395

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "azureOperationalInsightsBlockTelemetry": true,
    "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
    "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
    "connectAppBlockAutoLaunch": true,
    "maintenanceWindowBlocked": true,
    "maintenanceWindowDurationInHours": 0,
    "maintenanceWindowStartTime": "11:59:09.3130000",
    "miracastChannel": "one",
    "miracastBlocked": true,
    "miracastRequirePin": true,
    "settingsBlockMyMeetingsAndFiles": true,
    "settingsBlockSessionResume": true,
    "settingsBlockSigninSuggestions": true,
    "settingsDefaultVolume": 5,
    "settingsScreenTimeoutInMinutes": 14,
    "settingsSessionTimeoutInMinutes": 15,
    "settingsSleepTimeoutInMinutes": 13,
    "welcomeScreenBlockAutomaticWakeUp": true,
    "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
    "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
  }
}
```



