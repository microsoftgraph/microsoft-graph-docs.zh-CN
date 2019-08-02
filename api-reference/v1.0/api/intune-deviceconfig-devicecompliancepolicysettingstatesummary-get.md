---
title: 获取 deviceCompliancePolicySettingStateSummary
description: 读取 deviceCompliancePolicySettingStateSummary 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d2f0473643000010fefc385fec13394bf319d31e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017768"
---
# <a name="get-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="250e3-103">获取 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="250e3-103">Get deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="250e3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="250e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="250e3-105">读取 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="250e3-105">Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="250e3-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="250e3-106">Prerequisites</span></span>
<span data-ttu-id="250e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="250e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="250e3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="250e3-109">Permission type</span></span>|<span data-ttu-id="250e3-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="250e3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="250e3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="250e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="250e3-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="250e3-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="250e3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="250e3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="250e3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="250e3-114">Not supported.</span></span>|
|<span data-ttu-id="250e3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="250e3-115">Application</span></span>|<span data-ttu-id="250e3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="250e3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="250e3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="250e3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="250e3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="250e3-118">Optional query parameters</span></span>
<span data-ttu-id="250e3-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="250e3-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="250e3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="250e3-120">Request headers</span></span>
|<span data-ttu-id="250e3-121">标头</span><span class="sxs-lookup"><span data-stu-id="250e3-121">Header</span></span>|<span data-ttu-id="250e3-122">值</span><span class="sxs-lookup"><span data-stu-id="250e3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="250e3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="250e3-123">Authorization</span></span>|<span data-ttu-id="250e3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="250e3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="250e3-125">接受</span><span class="sxs-lookup"><span data-stu-id="250e3-125">Accept</span></span>|<span data-ttu-id="250e3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="250e3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="250e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="250e3-127">Request body</span></span>
<span data-ttu-id="250e3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="250e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="250e3-129">响应</span><span class="sxs-lookup"><span data-stu-id="250e3-129">Response</span></span>
<span data-ttu-id="250e3-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="250e3-130">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="250e3-131">示例</span><span class="sxs-lookup"><span data-stu-id="250e3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="250e3-132">请求</span><span class="sxs-lookup"><span data-stu-id="250e3-132">Request</span></span>
<span data-ttu-id="250e3-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="250e3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

### <a name="response"></a><span data-ttu-id="250e3-134">响应</span><span class="sxs-lookup"><span data-stu-id="250e3-134">Response</span></span>
<span data-ttu-id="250e3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="250e3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
    "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "platformType": "iOS",
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



