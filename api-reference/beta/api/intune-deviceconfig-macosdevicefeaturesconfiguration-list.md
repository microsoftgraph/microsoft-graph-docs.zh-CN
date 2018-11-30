---
title: 列出 macOSDeviceFeaturesConfigurations
description: 列出 macOSDeviceFeaturesConfiguration 对象的属性和关系。
ms.openlocfilehash: 883929b6cf12d9da7699c1402c966bee8b0a229a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045477"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="d2c6a-103">列出 macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="d2c6a-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="d2c6a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d2c6a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2c6a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2c6a-107">列出 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d2c6a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d2c6a-108">Prerequisites</span></span>
<span data-ttu-id="d2c6a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d2c6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2c6a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2c6a-111">Permission type</span></span>|<span data-ttu-id="d2c6a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d2c6a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2c6a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2c6a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2c6a-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2c6a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d2c6a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2c6a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2c6a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-116">Not supported.</span></span>|
|<span data-ttu-id="d2c6a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2c6a-117">Application</span></span>|<span data-ttu-id="d2c6a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2c6a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2c6a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d2c6a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2c6a-120">Request headers</span></span>
|<span data-ttu-id="d2c6a-121">标头</span><span class="sxs-lookup"><span data-stu-id="d2c6a-121">Header</span></span>|<span data-ttu-id="d2c6a-122">值</span><span class="sxs-lookup"><span data-stu-id="d2c6a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2c6a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2c6a-123">Authorization</span></span>|<span data-ttu-id="d2c6a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2c6a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d2c6a-125">Accept</span></span>|<span data-ttu-id="d2c6a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2c6a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2c6a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2c6a-127">Request body</span></span>
<span data-ttu-id="d2c6a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2c6a-129">响应</span><span class="sxs-lookup"><span data-stu-id="d2c6a-129">Response</span></span>
<span data-ttu-id="d2c6a-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2c6a-131">示例</span><span class="sxs-lookup"><span data-stu-id="d2c6a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d2c6a-132">请求</span><span class="sxs-lookup"><span data-stu-id="d2c6a-132">Request</span></span>
<span data-ttu-id="d2c6a-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d2c6a-134">响应</span><span class="sxs-lookup"><span data-stu-id="d2c6a-134">Response</span></span>
<span data-ttu-id="d2c6a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2c6a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 785

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
      "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
  ]
}
```





