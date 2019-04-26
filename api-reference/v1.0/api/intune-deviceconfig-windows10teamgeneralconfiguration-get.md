---
title: 获取 windows10TeamGeneralConfiguration
description: 读取 windows10TeamGeneralConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa44e6bdd190d560dd77ff8ed0316f21cbb39a8f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558102"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="367c4-103">获取 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="367c4-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="367c4-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="367c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="367c4-105">读取 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="367c4-105">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="367c4-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="367c4-106">Prerequisites</span></span>
<span data-ttu-id="367c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="367c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="367c4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="367c4-109">Permission type</span></span>|<span data-ttu-id="367c4-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="367c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="367c4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="367c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="367c4-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="367c4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="367c4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="367c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="367c4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="367c4-114">Not supported.</span></span>|
|<span data-ttu-id="367c4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="367c4-115">Application</span></span>|<span data-ttu-id="367c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="367c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="367c4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="367c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="367c4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="367c4-118">Optional query parameters</span></span>
<span data-ttu-id="367c4-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="367c4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="367c4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="367c4-120">Request headers</span></span>
|<span data-ttu-id="367c4-121">标头</span><span class="sxs-lookup"><span data-stu-id="367c4-121">Header</span></span>|<span data-ttu-id="367c4-122">值</span><span class="sxs-lookup"><span data-stu-id="367c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="367c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="367c4-123">Authorization</span></span>|<span data-ttu-id="367c4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="367c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="367c4-125">接受</span><span class="sxs-lookup"><span data-stu-id="367c4-125">Accept</span></span>|<span data-ttu-id="367c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="367c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="367c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="367c4-127">Request body</span></span>
<span data-ttu-id="367c4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="367c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="367c4-129">响应</span><span class="sxs-lookup"><span data-stu-id="367c4-129">Response</span></span>
<span data-ttu-id="367c4-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="367c4-130">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="367c4-131">示例</span><span class="sxs-lookup"><span data-stu-id="367c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="367c4-132">请求</span><span class="sxs-lookup"><span data-stu-id="367c4-132">Request</span></span>
<span data-ttu-id="367c4-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="367c4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="367c4-134">响应</span><span class="sxs-lookup"><span data-stu-id="367c4-134">Response</span></span>
<span data-ttu-id="367c4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="367c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



