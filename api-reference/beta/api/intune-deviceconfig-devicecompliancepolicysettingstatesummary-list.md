---
title: 列出 deviceCompliancePolicySettingStateSummaries
description: 列出 deviceCompliancePolicySettingStateSummary 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b6b87987629f926dd21f24c826125d5e058336e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949690"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="40af7-103">列出 deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="40af7-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="40af7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40af7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40af7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40af7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40af7-106">列出 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="40af7-106">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40af7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="40af7-107">Prerequisites</span></span>
<span data-ttu-id="40af7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40af7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40af7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="40af7-110">Permission type</span></span>|<span data-ttu-id="40af7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40af7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40af7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40af7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="40af7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40af7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40af7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40af7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40af7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="40af7-115">Not supported.</span></span>|
|<span data-ttu-id="40af7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="40af7-116">Application</span></span>|<span data-ttu-id="40af7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="40af7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40af7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40af7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="40af7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="40af7-119">Request headers</span></span>
|<span data-ttu-id="40af7-120">标头</span><span class="sxs-lookup"><span data-stu-id="40af7-120">Header</span></span>|<span data-ttu-id="40af7-121">值</span><span class="sxs-lookup"><span data-stu-id="40af7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40af7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="40af7-122">Authorization</span></span>|<span data-ttu-id="40af7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40af7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40af7-124">接受</span><span class="sxs-lookup"><span data-stu-id="40af7-124">Accept</span></span>|<span data-ttu-id="40af7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="40af7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40af7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="40af7-126">Request body</span></span>
<span data-ttu-id="40af7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40af7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40af7-128">响应</span><span class="sxs-lookup"><span data-stu-id="40af7-128">Response</span></span>
<span data-ttu-id="40af7-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="40af7-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40af7-130">示例</span><span class="sxs-lookup"><span data-stu-id="40af7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="40af7-131">请求</span><span class="sxs-lookup"><span data-stu-id="40af7-131">Request</span></span>
<span data-ttu-id="40af7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40af7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="40af7-133">响应</span><span class="sxs-lookup"><span data-stu-id="40af7-133">Response</span></span>
<span data-ttu-id="40af7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40af7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": [
    {
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
  ]
}
```





