---
title: 获取 deviceManagementPartner
description: 读取 deviceManagementPartner 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57eafe24c0739e98903d28b01e276e0ca070d07f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463633"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="b77b5-103">获取 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="b77b5-103">Get deviceManagementPartner</span></span>

<span data-ttu-id="b77b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b77b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b77b5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b77b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b77b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b77b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b77b5-107">读取 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b77b5-107">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b77b5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b77b5-108">Prerequisites</span></span>
<span data-ttu-id="b77b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b77b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b77b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b77b5-111">Permission type</span></span>|<span data-ttu-id="b77b5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b77b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b77b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b77b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b77b5-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b77b5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b77b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b77b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b77b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b77b5-116">Not supported.</span></span>|
|<span data-ttu-id="b77b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b77b5-117">Application</span></span>|<span data-ttu-id="b77b5-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b77b5-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b77b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b77b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b77b5-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b77b5-120">Optional query parameters</span></span>
<span data-ttu-id="b77b5-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b77b5-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b77b5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b77b5-122">Request headers</span></span>
|<span data-ttu-id="b77b5-123">标头</span><span class="sxs-lookup"><span data-stu-id="b77b5-123">Header</span></span>|<span data-ttu-id="b77b5-124">值</span><span class="sxs-lookup"><span data-stu-id="b77b5-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b77b5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b77b5-125">Authorization</span></span>|<span data-ttu-id="b77b5-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b77b5-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b77b5-127">接受</span><span class="sxs-lookup"><span data-stu-id="b77b5-127">Accept</span></span>|<span data-ttu-id="b77b5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b77b5-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b77b5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b77b5-129">Request body</span></span>
<span data-ttu-id="b77b5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b77b5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b77b5-131">响应</span><span class="sxs-lookup"><span data-stu-id="b77b5-131">Response</span></span>
<span data-ttu-id="b77b5-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b77b5-132">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b77b5-133">示例</span><span class="sxs-lookup"><span data-stu-id="b77b5-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b77b5-134">请求</span><span class="sxs-lookup"><span data-stu-id="b77b5-134">Request</span></span>
<span data-ttu-id="b77b5-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b77b5-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="b77b5-136">响应</span><span class="sxs-lookup"><span data-stu-id="b77b5-136">Response</span></span>
<span data-ttu-id="b77b5-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b77b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1005

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00",
    "groupsRequiringPartnerEnrollment": [
      {
        "@odata.type": "microsoft.graph.deviceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ]
  }
}
```



