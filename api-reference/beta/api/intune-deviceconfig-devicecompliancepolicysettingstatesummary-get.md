---
title: 获取 deviceCompliancePolicySettingStateSummary
description: 读取 deviceCompliancePolicySettingStateSummary 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8c23d0dab9f4a09977f12014d2c91c4586eea1b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927732"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="f6670-103">获取 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="f6670-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="f6670-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6670-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6670-106">读取 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f6670-106">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6670-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6670-107">Prerequisites</span></span>
<span data-ttu-id="f6670-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6670-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6670-110">Permission type</span></span>|<span data-ttu-id="f6670-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f6670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6670-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6670-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6670-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f6670-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6670-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6670-115">Not supported.</span></span>|
|<span data-ttu-id="f6670-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6670-116">Application</span></span>|<span data-ttu-id="f6670-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6670-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6670-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6670-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f6670-119">Optional query parameters</span></span>
<span data-ttu-id="f6670-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f6670-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6670-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6670-121">Request headers</span></span>
|<span data-ttu-id="f6670-122">标头</span><span class="sxs-lookup"><span data-stu-id="f6670-122">Header</span></span>|<span data-ttu-id="f6670-123">值</span><span class="sxs-lookup"><span data-stu-id="f6670-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6670-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6670-124">Authorization</span></span>|<span data-ttu-id="f6670-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6670-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6670-126">接受</span><span class="sxs-lookup"><span data-stu-id="f6670-126">Accept</span></span>|<span data-ttu-id="f6670-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6670-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6670-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6670-128">Request body</span></span>
<span data-ttu-id="f6670-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6670-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6670-130">响应</span><span class="sxs-lookup"><span data-stu-id="f6670-130">Response</span></span>
<span data-ttu-id="f6670-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6670-131">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6670-132">示例</span><span class="sxs-lookup"><span data-stu-id="f6670-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6670-133">请求</span><span class="sxs-lookup"><span data-stu-id="f6670-133">Request</span></span>
<span data-ttu-id="f6670-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6670-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="f6670-135">响应</span><span class="sxs-lookup"><span data-stu-id="f6670-135">Response</span></span>
<span data-ttu-id="f6670-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6670-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
    "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "platformType": "androidForWork",
    "unknownDeviceCount": 2,
    "notApplicableDeviceCount": 8,
    "compliantDeviceCount": 4,
    "remediatedDeviceCount": 5,
    "nonCompliantDeviceCount": 7,
    "errorDeviceCount": 0,
    "conflictDeviceCount": 3
  }
}
```




