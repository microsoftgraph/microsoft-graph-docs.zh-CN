---
title: 获取 complianceManagementPartner
description: 读取 complianceManagementPartner 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1f88054b46668016b3fda0e7e7733479863ec163
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38086695"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="8691d-103">获取 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8691d-103">Get complianceManagementPartner</span></span>

> <span data-ttu-id="8691d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8691d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8691d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8691d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8691d-106">读取[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8691d-106">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8691d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8691d-107">Prerequisites</span></span>
<span data-ttu-id="8691d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8691d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8691d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8691d-110">Permission type</span></span>|<span data-ttu-id="8691d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8691d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8691d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8691d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8691d-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8691d-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8691d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8691d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8691d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8691d-115">Not supported.</span></span>|
|<span data-ttu-id="8691d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8691d-116">Application</span></span>|<span data-ttu-id="8691d-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8691d-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8691d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8691d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8691d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8691d-119">Optional query parameters</span></span>
<span data-ttu-id="8691d-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8691d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8691d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8691d-121">Request headers</span></span>
|<span data-ttu-id="8691d-122">标头</span><span class="sxs-lookup"><span data-stu-id="8691d-122">Header</span></span>|<span data-ttu-id="8691d-123">值</span><span class="sxs-lookup"><span data-stu-id="8691d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8691d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8691d-124">Authorization</span></span>|<span data-ttu-id="8691d-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8691d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8691d-126">接受</span><span class="sxs-lookup"><span data-stu-id="8691d-126">Accept</span></span>|<span data-ttu-id="8691d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8691d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8691d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8691d-128">Request body</span></span>
<span data-ttu-id="8691d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8691d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8691d-130">响应</span><span class="sxs-lookup"><span data-stu-id="8691d-130">Response</span></span>
<span data-ttu-id="8691d-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8691d-131">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8691d-132">示例</span><span class="sxs-lookup"><span data-stu-id="8691d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8691d-133">请求</span><span class="sxs-lookup"><span data-stu-id="8691d-133">Request</span></span>
<span data-ttu-id="8691d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8691d-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="8691d-135">响应</span><span class="sxs-lookup"><span data-stu-id="8691d-135">Response</span></span>
<span data-ttu-id="8691d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8691d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

{
  "value": {
    "@odata.type": "#microsoft.graph.complianceManagementPartner",
    "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "displayName": "Display Name value",
    "macOsOnboarded": true,
    "windowsOnboarded": true,
    "androidOnboarded": true,
    "iosOnboarded": true,
    "macOsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ],
    "windowsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ],
    "androidEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ],
    "iosEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
        }
      }
    ]
  }
}
```






