---
title: 列出 complianceManagementPartners
description: 列出 complianceManagementPartner 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 91f43342fa21cad981663578ab0c98c3a2e1aefb
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744115"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="d5028-103">列出 complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="d5028-103">List complianceManagementPartners</span></span>

<span data-ttu-id="d5028-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5028-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5028-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5028-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5028-106">列出[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5028-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5028-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5028-107">Prerequisites</span></span>
<span data-ttu-id="d5028-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d5028-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d5028-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5028-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5028-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5028-110">Permission type</span></span>|<span data-ttu-id="d5028-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5028-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5028-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5028-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d5028-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5028-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d5028-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5028-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5028-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5028-115">Not supported.</span></span>|
|<span data-ttu-id="d5028-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5028-116">Application</span></span>|<span data-ttu-id="d5028-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5028-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5028-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5028-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="d5028-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5028-119">Request headers</span></span>
|<span data-ttu-id="d5028-120">标头</span><span class="sxs-lookup"><span data-stu-id="d5028-120">Header</span></span>|<span data-ttu-id="d5028-121">值</span><span class="sxs-lookup"><span data-stu-id="d5028-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5028-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5028-122">Authorization</span></span>|<span data-ttu-id="d5028-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5028-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5028-124">接受</span><span class="sxs-lookup"><span data-stu-id="d5028-124">Accept</span></span>|<span data-ttu-id="d5028-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d5028-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5028-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5028-126">Request body</span></span>
<span data-ttu-id="d5028-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5028-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5028-128">响应</span><span class="sxs-lookup"><span data-stu-id="d5028-128">Response</span></span>
<span data-ttu-id="d5028-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d5028-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5028-130">示例</span><span class="sxs-lookup"><span data-stu-id="d5028-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5028-131">请求</span><span class="sxs-lookup"><span data-stu-id="d5028-131">Request</span></span>
<span data-ttu-id="d5028-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5028-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="d5028-133">响应</span><span class="sxs-lookup"><span data-stu-id="d5028-133">Response</span></span>
<span data-ttu-id="d5028-134">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d5028-134">Here is an example of the response.</span></span> <span data-ttu-id="d5028-135">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d5028-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5028-136">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d5028-136">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1192

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.complianceManagementPartner",
      "id": "d6d46d0d-6d0d-d6d4-0d6d-d4d60d6dd4d6",
      "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
      "partnerState": "unavailable",
      "displayName": "Display Name value",
      "macOsOnboarded": true,
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
  ]
}
```



