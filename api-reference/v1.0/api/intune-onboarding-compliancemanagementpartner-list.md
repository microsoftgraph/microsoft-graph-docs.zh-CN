---
title: 列出 complianceManagementPartners
description: 列出 complianceManagementPartner 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5a67f425e110def02b995b9fe24b218b35f28e88
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759063"
---
# <a name="list-compliancemanagementpartners"></a><span data-ttu-id="136df-103">列出 complianceManagementPartners</span><span class="sxs-lookup"><span data-stu-id="136df-103">List complianceManagementPartners</span></span>

<span data-ttu-id="136df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="136df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="136df-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="136df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="136df-106">列出 [complianceManagementPartner 对象的属性和](../resources/intune-onboarding-compliancemanagementpartner.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="136df-106">List properties and relationships of the [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="136df-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="136df-107">Prerequisites</span></span>
<span data-ttu-id="136df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="136df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="136df-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="136df-110">Permission type</span></span>|<span data-ttu-id="136df-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="136df-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="136df-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="136df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="136df-113">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136df-113">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="136df-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="136df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="136df-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="136df-115">Not supported.</span></span>|
|<span data-ttu-id="136df-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="136df-116">Application</span></span>|<span data-ttu-id="136df-117">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="136df-117">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="136df-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="136df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/complianceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="136df-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="136df-119">Request headers</span></span>
|<span data-ttu-id="136df-120">标头</span><span class="sxs-lookup"><span data-stu-id="136df-120">Header</span></span>|<span data-ttu-id="136df-121">值</span><span class="sxs-lookup"><span data-stu-id="136df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="136df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="136df-122">Authorization</span></span>|<span data-ttu-id="136df-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="136df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="136df-124">接受</span><span class="sxs-lookup"><span data-stu-id="136df-124">Accept</span></span>|<span data-ttu-id="136df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="136df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="136df-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="136df-126">Request body</span></span>
<span data-ttu-id="136df-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="136df-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="136df-128">响应</span><span class="sxs-lookup"><span data-stu-id="136df-128">Response</span></span>
<span data-ttu-id="136df-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="136df-129">If successful, this method returns a `200 OK` response code and a collection of [complianceManagementPartner](../resources/intune-onboarding-compliancemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="136df-130">示例</span><span class="sxs-lookup"><span data-stu-id="136df-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="136df-131">请求</span><span class="sxs-lookup"><span data-stu-id="136df-131">Request</span></span>
<span data-ttu-id="136df-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="136df-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/complianceManagementPartners
```

### <a name="response"></a><span data-ttu-id="136df-133">响应</span><span class="sxs-lookup"><span data-stu-id="136df-133">Response</span></span>
<span data-ttu-id="136df-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="136df-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

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
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "androidEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ],
      "iosEnrollmentAssignments": [
        {
          "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment",
          "target": {
            "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
            "collectionId": "Collection Id value"
          }
        }
      ]
    }
  ]
}
```




