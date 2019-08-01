---
title: 获取 settingStateDeviceSummary
description: 读取 settingStateDeviceSummary 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e703e1744089f20c53c99f303d10618b3f4021af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017054"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="5f0be-103">获取 settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5f0be-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="5f0be-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f0be-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f0be-105">读取 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f0be-105">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f0be-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f0be-106">Prerequisites</span></span>
<span data-ttu-id="5f0be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f0be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f0be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f0be-109">Permission type</span></span>|<span data-ttu-id="5f0be-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f0be-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f0be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f0be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f0be-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f0be-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f0be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f0be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f0be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f0be-114">Not supported.</span></span>|
|<span data-ttu-id="5f0be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f0be-115">Application</span></span>|<span data-ttu-id="5f0be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f0be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f0be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f0be-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f0be-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f0be-118">Optional query parameters</span></span>
<span data-ttu-id="5f0be-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f0be-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f0be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f0be-120">Request headers</span></span>
|<span data-ttu-id="5f0be-121">标头</span><span class="sxs-lookup"><span data-stu-id="5f0be-121">Header</span></span>|<span data-ttu-id="5f0be-122">值</span><span class="sxs-lookup"><span data-stu-id="5f0be-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f0be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f0be-123">Authorization</span></span>|<span data-ttu-id="5f0be-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f0be-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f0be-125">接受</span><span class="sxs-lookup"><span data-stu-id="5f0be-125">Accept</span></span>|<span data-ttu-id="5f0be-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f0be-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f0be-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f0be-127">Request body</span></span>
<span data-ttu-id="5f0be-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f0be-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f0be-129">响应</span><span class="sxs-lookup"><span data-stu-id="5f0be-129">Response</span></span>
<span data-ttu-id="5f0be-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f0be-130">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f0be-131">示例</span><span class="sxs-lookup"><span data-stu-id="5f0be-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f0be-132">请求</span><span class="sxs-lookup"><span data-stu-id="5f0be-132">Request</span></span>
<span data-ttu-id="5f0be-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f0be-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="5f0be-134">响应</span><span class="sxs-lookup"><span data-stu-id="5f0be-134">Response</span></span>
<span data-ttu-id="5f0be-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f0be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
    "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
    "settingName": "Setting Name value",
    "instancePath": "Instance Path value",
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



