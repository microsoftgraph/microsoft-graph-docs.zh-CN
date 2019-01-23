---
title: 获取 managedAppConfiguration
description: 读取 managedAppConfiguration 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ccc0f3f7a2799d1b9e21ce53724fccd9eb4996c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404468"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="80b38-103">获取 managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="80b38-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="80b38-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="80b38-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80b38-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80b38-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80b38-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80b38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80b38-107">读取 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="80b38-107">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80b38-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="80b38-108">Prerequisites</span></span>
<span data-ttu-id="80b38-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="80b38-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="80b38-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80b38-111">Permission type</span></span>|<span data-ttu-id="80b38-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80b38-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80b38-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80b38-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80b38-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="80b38-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="80b38-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80b38-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80b38-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80b38-116">Not supported.</span></span>|
|<span data-ttu-id="80b38-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80b38-117">Application</span></span>|<span data-ttu-id="80b38-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="80b38-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80b38-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80b38-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="80b38-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="80b38-120">Optional query parameters</span></span>
<span data-ttu-id="80b38-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="80b38-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="80b38-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="80b38-122">Request headers</span></span>
|<span data-ttu-id="80b38-123">标头</span><span class="sxs-lookup"><span data-stu-id="80b38-123">Header</span></span>|<span data-ttu-id="80b38-124">值</span><span class="sxs-lookup"><span data-stu-id="80b38-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80b38-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="80b38-125">Authorization</span></span>|<span data-ttu-id="80b38-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80b38-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80b38-127">Accept</span><span class="sxs-lookup"><span data-stu-id="80b38-127">Accept</span></span>|<span data-ttu-id="80b38-128">application/json</span><span class="sxs-lookup"><span data-stu-id="80b38-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80b38-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="80b38-129">Request body</span></span>
<span data-ttu-id="80b38-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="80b38-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80b38-131">响应</span><span class="sxs-lookup"><span data-stu-id="80b38-131">Response</span></span>
<span data-ttu-id="80b38-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80b38-132">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80b38-133">示例</span><span class="sxs-lookup"><span data-stu-id="80b38-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="80b38-134">请求</span><span class="sxs-lookup"><span data-stu-id="80b38-134">Request</span></span>
<span data-ttu-id="80b38-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80b38-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="80b38-136">响应</span><span class="sxs-lookup"><span data-stu-id="80b38-136">Response</span></span>
<span data-ttu-id="80b38-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80b38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 618

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```




