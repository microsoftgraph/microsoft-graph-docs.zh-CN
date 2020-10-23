---
title: 列出 deviceCompliancePolicySettingStateSummaries
description: 列出 deviceCompliancePolicySettingStateSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4f7de2ed287062b3b6878ff3b01f837c7980609
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733844"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="bedf2-103">列出 deviceCompliancePolicySettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="bedf2-103">List deviceCompliancePolicySettingStateSummaries</span></span>

<span data-ttu-id="bedf2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bedf2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bedf2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bedf2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bedf2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bedf2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bedf2-107">列出 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bedf2-107">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bedf2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bedf2-108">Prerequisites</span></span>
<span data-ttu-id="bedf2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bedf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bedf2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bedf2-111">Permission type</span></span>|<span data-ttu-id="bedf2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bedf2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bedf2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bedf2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bedf2-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bedf2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bedf2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bedf2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bedf2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bedf2-116">Not supported.</span></span>|
|<span data-ttu-id="bedf2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bedf2-117">Application</span></span>|<span data-ttu-id="bedf2-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bedf2-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bedf2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bedf2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="bedf2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bedf2-120">Request headers</span></span>
|<span data-ttu-id="bedf2-121">标头</span><span class="sxs-lookup"><span data-stu-id="bedf2-121">Header</span></span>|<span data-ttu-id="bedf2-122">值</span><span class="sxs-lookup"><span data-stu-id="bedf2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bedf2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bedf2-123">Authorization</span></span>|<span data-ttu-id="bedf2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bedf2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bedf2-125">接受</span><span class="sxs-lookup"><span data-stu-id="bedf2-125">Accept</span></span>|<span data-ttu-id="bedf2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bedf2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bedf2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bedf2-127">Request body</span></span>
<span data-ttu-id="bedf2-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bedf2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bedf2-129">响应</span><span class="sxs-lookup"><span data-stu-id="bedf2-129">Response</span></span>
<span data-ttu-id="bedf2-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bedf2-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bedf2-131">示例</span><span class="sxs-lookup"><span data-stu-id="bedf2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bedf2-132">请求</span><span class="sxs-lookup"><span data-stu-id="bedf2-132">Request</span></span>
<span data-ttu-id="bedf2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bedf2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="bedf2-134">响应</span><span class="sxs-lookup"><span data-stu-id="bedf2-134">Response</span></span>
<span data-ttu-id="bedf2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bedf2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





