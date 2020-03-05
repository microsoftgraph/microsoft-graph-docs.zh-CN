---
title: 列出 complianceManagementPartners
description: 列出 complianceManagementPartner 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 152ec1bee04a25a3d63ff34f58b63a1447d42946
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42462444"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="53e13-103">列出 complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="53e13-103">List complianceManagementPartners</span></span>

<span data-ttu-id="53e13-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="53e13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53e13-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53e13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53e13-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53e13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e13-107">列出[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53e13-107">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53e13-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="53e13-108">Prerequisites</span></span>
<span data-ttu-id="53e13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53e13-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53e13-111">Permission type</span></span>|<span data-ttu-id="53e13-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53e13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53e13-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53e13-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53e13-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="53e13-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="53e13-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53e13-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53e13-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53e13-116">Not supported.</span></span>|
|<span data-ttu-id="53e13-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53e13-117">Application</span></span>|<span data-ttu-id="53e13-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="53e13-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53e13-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53e13-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="53e13-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53e13-120">Request headers</span></span>
|<span data-ttu-id="53e13-121">标头</span><span class="sxs-lookup"><span data-stu-id="53e13-121">Header</span></span>|<span data-ttu-id="53e13-122">值</span><span class="sxs-lookup"><span data-stu-id="53e13-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53e13-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53e13-123">Authorization</span></span>|<span data-ttu-id="53e13-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53e13-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53e13-125">接受</span><span class="sxs-lookup"><span data-stu-id="53e13-125">Accept</span></span>|<span data-ttu-id="53e13-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53e13-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53e13-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53e13-127">Request body</span></span>
<span data-ttu-id="53e13-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53e13-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53e13-129">响应</span><span class="sxs-lookup"><span data-stu-id="53e13-129">Response</span></span>
<span data-ttu-id="53e13-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="53e13-130">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53e13-131">示例</span><span class="sxs-lookup"><span data-stu-id="53e13-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="53e13-132">请求</span><span class="sxs-lookup"><span data-stu-id="53e13-132">Request</span></span>
<span data-ttu-id="53e13-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53e13-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="53e13-134">响应</span><span class="sxs-lookup"><span data-stu-id="53e13-134">Response</span></span>
<span data-ttu-id="53e13-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53e13-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1490

{
  "value": [
    {
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
  ]
}
```





