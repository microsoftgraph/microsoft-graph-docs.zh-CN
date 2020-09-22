---
title: 列出 deviceComplianceSettingStates
description: 列出 deviceComplianceSettingState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05628cd87448595883ee0866eb832e3ac7ad3094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48011667"
---
# <a name="list-devicecompliancesettingstates"></a><span data-ttu-id="b9e6f-103">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="b9e6f-103">List deviceComplianceSettingStates</span></span>

<span data-ttu-id="b9e6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9e6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9e6f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9e6f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9e6f-107">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-107">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9e6f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9e6f-108">Prerequisites</span></span>
<span data-ttu-id="b9e6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9e6f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9e6f-111">Permission type</span></span>|<span data-ttu-id="b9e6f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9e6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9e6f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9e6f-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e6f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9e6f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9e6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9e6f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-116">Not supported.</span></span>|
|<span data-ttu-id="b9e6f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9e6f-117">Application</span></span>|<span data-ttu-id="b9e6f-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9e6f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9e6f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9e6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="b9e6f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9e6f-120">Request headers</span></span>
|<span data-ttu-id="b9e6f-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9e6f-121">Header</span></span>|<span data-ttu-id="b9e6f-122">值</span><span class="sxs-lookup"><span data-stu-id="b9e6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9e6f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9e6f-123">Authorization</span></span>|<span data-ttu-id="b9e6f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9e6f-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9e6f-125">Accept</span></span>|<span data-ttu-id="b9e6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9e6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9e6f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9e6f-127">Request body</span></span>
<span data-ttu-id="b9e6f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9e6f-129">响应</span><span class="sxs-lookup"><span data-stu-id="b9e6f-129">Response</span></span>
<span data-ttu-id="b9e6f-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-130">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9e6f-131">示例</span><span class="sxs-lookup"><span data-stu-id="b9e6f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9e6f-132">请求</span><span class="sxs-lookup"><span data-stu-id="b9e6f-132">Request</span></span>
<span data-ttu-id="b9e6f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates
```

### <a name="response"></a><span data-ttu-id="b9e6f-134">响应</span><span class="sxs-lookup"><span data-stu-id="b9e6f-134">Response</span></span>
<span data-ttu-id="b9e6f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9e6f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
      "id": "9905f955-f955-9905-55f9-059955f90599",
      "platformType": "windowsRT",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "deviceModel": "Device Model value",
      "state": "notApplicable",
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
    }
  ]
}
```






