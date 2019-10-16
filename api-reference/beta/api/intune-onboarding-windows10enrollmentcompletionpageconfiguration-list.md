---
title: 列出 windows10EnrollmentCompletionPageConfigurations
description: 列出 windows10EnrollmentCompletionPageConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ed0ebb28d599ececd0e60355d74be073fa5031b1
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536530"
---
# <a name="list-windows10enrollmentcompletionpageconfigurations"></a><span data-ttu-id="a4d68-103">列出 windows10EnrollmentCompletionPageConfigurations</span><span class="sxs-lookup"><span data-stu-id="a4d68-103">List windows10EnrollmentCompletionPageConfigurations</span></span>

> <span data-ttu-id="a4d68-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4d68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4d68-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4d68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4d68-106">列出[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4d68-106">List properties and relationships of the [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4d68-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4d68-107">Prerequisites</span></span>
<span data-ttu-id="a4d68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4d68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4d68-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4d68-110">Permission type</span></span>|<span data-ttu-id="a4d68-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4d68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4d68-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4d68-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4d68-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a4d68-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4d68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4d68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4d68-115">Not supported.</span></span>|
|<span data-ttu-id="a4d68-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4d68-116">Application</span></span>|<span data-ttu-id="a4d68-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4d68-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4d68-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4d68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4d68-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4d68-119">Request headers</span></span>
|<span data-ttu-id="a4d68-120">标头</span><span class="sxs-lookup"><span data-stu-id="a4d68-120">Header</span></span>|<span data-ttu-id="a4d68-121">值</span><span class="sxs-lookup"><span data-stu-id="a4d68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4d68-122">授权</span><span class="sxs-lookup"><span data-stu-id="a4d68-122">Authorization</span></span>|<span data-ttu-id="a4d68-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4d68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4d68-124">接受</span><span class="sxs-lookup"><span data-stu-id="a4d68-124">Accept</span></span>|<span data-ttu-id="a4d68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4d68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4d68-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4d68-126">Request body</span></span>
<span data-ttu-id="a4d68-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4d68-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4d68-128">响应</span><span class="sxs-lookup"><span data-stu-id="a4d68-128">Response</span></span>
<span data-ttu-id="a4d68-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a4d68-129">If successful, this method returns a `200 OK` response code and a collection of [windows10EnrollmentCompletionPageConfiguration](../resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4d68-130">示例</span><span class="sxs-lookup"><span data-stu-id="a4d68-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4d68-131">请求</span><span class="sxs-lookup"><span data-stu-id="a4d68-131">Request</span></span>
<span data-ttu-id="a4d68-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4d68-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="a4d68-133">响应</span><span class="sxs-lookup"><span data-stu-id="a4d68-133">Response</span></span>
<span data-ttu-id="a4d68-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4d68-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 969

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfiguration",
      "id": "77bf8248-8248-77bf-4882-bf774882bf77",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "showInstallationProgress": true,
      "blockDeviceSetupRetryByUser": true,
      "allowDeviceResetOnInstallFailure": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true,
      "selectedMobileAppIds": [
        "Selected Mobile App Ids value"
      ],
      "trackInstallProgressForAutopilotOnly": true,
      "disableUserStatusTrackingAfterFirstUser": true
    }
  ]
}
```






