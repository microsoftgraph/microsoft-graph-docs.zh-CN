---
title: 获取 deviceCompliancePolicyDeviceStateSummary
description: 读取 deviceCompliancePolicyDeviceStateSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f857204a79a8acb774d70038026b7d5d334f1db1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130180"
---
# <a name="get-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="b54b0-103">获取 deviceCompliancePolicyDeviceStateSummary</span><span class="sxs-lookup"><span data-stu-id="b54b0-103">Get deviceCompliancePolicyDeviceStateSummary</span></span>

<span data-ttu-id="b54b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b54b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b54b0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b54b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b54b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b54b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b54b0-107">读取 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b54b0-107">Read properties and relationships of the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b54b0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b54b0-108">Prerequisites</span></span>
<span data-ttu-id="b54b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b54b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b54b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b54b0-111">Permission type</span></span>|<span data-ttu-id="b54b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b54b0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b54b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b54b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b54b0-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b54b0-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b54b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b54b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b54b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b54b0-116">Not supported.</span></span>|
|<span data-ttu-id="b54b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b54b0-117">Application</span></span>|<span data-ttu-id="b54b0-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b54b0-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b54b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b54b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b54b0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b54b0-120">Optional query parameters</span></span>
<span data-ttu-id="b54b0-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b54b0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b54b0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b54b0-122">Request headers</span></span>
|<span data-ttu-id="b54b0-123">标头</span><span class="sxs-lookup"><span data-stu-id="b54b0-123">Header</span></span>|<span data-ttu-id="b54b0-124">值</span><span class="sxs-lookup"><span data-stu-id="b54b0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b54b0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b54b0-125">Authorization</span></span>|<span data-ttu-id="b54b0-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b54b0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b54b0-127">接受</span><span class="sxs-lookup"><span data-stu-id="b54b0-127">Accept</span></span>|<span data-ttu-id="b54b0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b54b0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b54b0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b54b0-129">Request body</span></span>
<span data-ttu-id="b54b0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b54b0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b54b0-131">响应</span><span class="sxs-lookup"><span data-stu-id="b54b0-131">Response</span></span>
<span data-ttu-id="b54b0-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b54b0-132">If successful, this method returns a `200 OK` response code and [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b54b0-133">示例</span><span class="sxs-lookup"><span data-stu-id="b54b0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b54b0-134">请求</span><span class="sxs-lookup"><span data-stu-id="b54b0-134">Request</span></span>
<span data-ttu-id="b54b0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b54b0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

### <a name="response"></a><span data-ttu-id="b54b0-136">响应</span><span class="sxs-lookup"><span data-stu-id="b54b0-136">Response</span></span>
<span data-ttu-id="b54b0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b54b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 439

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
    "inGracePeriodCount": 2,
    "configManagerCount": 2,
    "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
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




