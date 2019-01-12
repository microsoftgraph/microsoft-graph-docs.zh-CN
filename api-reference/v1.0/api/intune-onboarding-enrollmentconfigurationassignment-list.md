---
title: 列出 enrollmentConfigurationAssignments
description: 列出 enrollmentConfigurationAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1750e3c0f8f712105cdada13a1b74f8e579c3bdd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981390"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="de2ce-103">列出 enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="de2ce-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="de2ce-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="de2ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de2ce-105">列出 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="de2ce-105">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de2ce-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="de2ce-106">Prerequisites</span></span>
<span data-ttu-id="de2ce-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="de2ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de2ce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="de2ce-109">Permission type</span></span>|<span data-ttu-id="de2ce-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de2ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de2ce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de2ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de2ce-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="de2ce-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="de2ce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de2ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de2ce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="de2ce-114">Not supported.</span></span>|
|<span data-ttu-id="de2ce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="de2ce-115">Application</span></span>|<span data-ttu-id="de2ce-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de2ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de2ce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de2ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="de2ce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="de2ce-118">Request headers</span></span>
|<span data-ttu-id="de2ce-119">标头</span><span class="sxs-lookup"><span data-stu-id="de2ce-119">Header</span></span>|<span data-ttu-id="de2ce-120">值</span><span class="sxs-lookup"><span data-stu-id="de2ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de2ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de2ce-121">Authorization</span></span>|<span data-ttu-id="de2ce-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de2ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de2ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="de2ce-123">Accept</span></span>|<span data-ttu-id="de2ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de2ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de2ce-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="de2ce-125">Request body</span></span>
<span data-ttu-id="de2ce-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="de2ce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de2ce-127">响应</span><span class="sxs-lookup"><span data-stu-id="de2ce-127">Response</span></span>
<span data-ttu-id="de2ce-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="de2ce-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de2ce-129">示例</span><span class="sxs-lookup"><span data-stu-id="de2ce-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="de2ce-130">请求</span><span class="sxs-lookup"><span data-stu-id="de2ce-130">Request</span></span>
<span data-ttu-id="de2ce-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de2ce-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="de2ce-132">响应</span><span class="sxs-lookup"><span data-stu-id="de2ce-132">Response</span></span>
<span data-ttu-id="de2ce-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de2ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



