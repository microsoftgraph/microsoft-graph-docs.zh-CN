---
title: 获取 appleDeviceFeaturesConfigurationBase
description: 读取 appleDeviceFeaturesConfigurationBase 对象的属性和关系。
ms.openlocfilehash: 1f2058f7f38f1033e243f635a7cc17245a7e7b26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048474"
---
# <a name="get-appledevicefeaturesconfigurationbase"></a><span data-ttu-id="d332e-103">获取 appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="d332e-103">Get appleDeviceFeaturesConfigurationBase</span></span>

> <span data-ttu-id="d332e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d332e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d332e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d332e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d332e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d332e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d332e-107">读取 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d332e-107">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d332e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d332e-108">Prerequisites</span></span>
<span data-ttu-id="d332e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d332e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d332e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d332e-111">Permission type</span></span>|<span data-ttu-id="d332e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d332e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d332e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d332e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d332e-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d332e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d332e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d332e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d332e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d332e-116">Not supported.</span></span>|
|<span data-ttu-id="d332e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d332e-117">Application</span></span>|<span data-ttu-id="d332e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d332e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d332e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d332e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d332e-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d332e-120">Optional query parameters</span></span>
<span data-ttu-id="d332e-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d332e-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d332e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d332e-122">Request headers</span></span>
|<span data-ttu-id="d332e-123">标头</span><span class="sxs-lookup"><span data-stu-id="d332e-123">Header</span></span>|<span data-ttu-id="d332e-124">值</span><span class="sxs-lookup"><span data-stu-id="d332e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d332e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d332e-125">Authorization</span></span>|<span data-ttu-id="d332e-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d332e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d332e-127">Accept</span><span class="sxs-lookup"><span data-stu-id="d332e-127">Accept</span></span>|<span data-ttu-id="d332e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d332e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d332e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d332e-129">Request body</span></span>
<span data-ttu-id="d332e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d332e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d332e-131">响应</span><span class="sxs-lookup"><span data-stu-id="d332e-131">Response</span></span>
<span data-ttu-id="d332e-132">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d332e-132">If successful, this method returns a `200 OK` response code and [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d332e-133">示例</span><span class="sxs-lookup"><span data-stu-id="d332e-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d332e-134">请求</span><span class="sxs-lookup"><span data-stu-id="d332e-134">Request</span></span>
<span data-ttu-id="d332e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d332e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d332e-136">响应</span><span class="sxs-lookup"><span data-stu-id="d332e-136">Response</span></span>
<span data-ttu-id="d332e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d332e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 735

{
  "value": {
    "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
    "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination",
        "ipAddress": "Ip Address value",
        "resourcePath": "Resource Path value",
        "port": 4,
        "forceTls": true
      }
    ]
  }
}
```





