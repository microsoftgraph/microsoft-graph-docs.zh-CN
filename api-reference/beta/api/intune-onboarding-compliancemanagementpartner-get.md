---
title: 获取 complianceManagementPartner
description: 读取 complianceManagementPartner 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b4830f22ff6b37c279a348e02f115e7f98a461c
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791845"
---
# <a name="get-compliancemanagementpartner"></a><span data-ttu-id="46830-103">获取 complianceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="46830-103">Get complianceManagementPartner</span></span>

<span data-ttu-id="46830-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46830-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="46830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46830-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46830-107">读取[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="46830-107">Read properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46830-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="46830-108">Prerequisites</span></span>
<span data-ttu-id="46830-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="46830-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="46830-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46830-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46830-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="46830-111">Permission type</span></span>|<span data-ttu-id="46830-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="46830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46830-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46830-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46830-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46830-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="46830-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46830-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46830-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="46830-116">Not supported.</span></span>|
|<span data-ttu-id="46830-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="46830-117">Application</span></span>|<span data-ttu-id="46830-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="46830-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46830-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46830-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46830-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46830-120">Optional query parameters</span></span>
<span data-ttu-id="46830-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="46830-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46830-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="46830-122">Request headers</span></span>
|<span data-ttu-id="46830-123">标头</span><span class="sxs-lookup"><span data-stu-id="46830-123">Header</span></span>|<span data-ttu-id="46830-124">值</span><span class="sxs-lookup"><span data-stu-id="46830-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46830-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="46830-125">Authorization</span></span>|<span data-ttu-id="46830-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="46830-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46830-127">接受</span><span class="sxs-lookup"><span data-stu-id="46830-127">Accept</span></span>|<span data-ttu-id="46830-128">application/json</span><span class="sxs-lookup"><span data-stu-id="46830-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46830-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="46830-129">Request body</span></span>
<span data-ttu-id="46830-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46830-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46830-131">响应</span><span class="sxs-lookup"><span data-stu-id="46830-131">Response</span></span>
<span data-ttu-id="46830-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象。</span><span class="sxs-lookup"><span data-stu-id="46830-132">If successful, this method returns a `200 OK` response code and [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46830-133">示例</span><span class="sxs-lookup"><span data-stu-id="46830-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="46830-134">请求</span><span class="sxs-lookup"><span data-stu-id="46830-134">Request</span></span>
<span data-ttu-id="46830-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="46830-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners/{complianceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="46830-136">响应</span><span class="sxs-lookup"><span data-stu-id="46830-136">Response</span></span>
<span data-ttu-id="46830-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="46830-137">Here is an example of the response.</span></span> <span data-ttu-id="46830-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="46830-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="46830-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="46830-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2110

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
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ],
    "windowsEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ],
    "androidEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ],
    "iosEnrollmentAssignments": [
      {
        "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
        "target": {
          "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
          "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
          "deviceAndAppManagementAssignmentFilterType": "include"
        }
      }
    ]
  }
}
```



