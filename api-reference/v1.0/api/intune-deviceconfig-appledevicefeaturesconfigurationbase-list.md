---
title: 列出 appleDeviceFeaturesConfigurationBases
description: 列出 appleDeviceFeaturesConfigurationBase 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: 969e3eb4067a88302311e8f7680d035567f4f8ec
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332065"
---
# <a name="list-appledevicefeaturesconfigurationbases"></a><span data-ttu-id="7dd1d-103">列出 appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="7dd1d-103">List appleDeviceFeaturesConfigurationBases</span></span>

> <span data-ttu-id="7dd1d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dd1d-105">列出 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-105">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7dd1d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dd1d-106">Prerequisites</span></span>
<span data-ttu-id="7dd1d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7dd1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dd1d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dd1d-109">Permission type</span></span>|<span data-ttu-id="7dd1d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dd1d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dd1d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dd1d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7dd1d-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7dd1d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7dd1d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dd1d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dd1d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-114">Not supported.</span></span>|
|<span data-ttu-id="7dd1d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dd1d-115">Application</span></span>|<span data-ttu-id="7dd1d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dd1d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dd1d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7dd1d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dd1d-118">Request headers</span></span>
|<span data-ttu-id="7dd1d-119">标头</span><span class="sxs-lookup"><span data-stu-id="7dd1d-119">Header</span></span>|<span data-ttu-id="7dd1d-120">值</span><span class="sxs-lookup"><span data-stu-id="7dd1d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dd1d-121">授权</span><span class="sxs-lookup"><span data-stu-id="7dd1d-121">Authorization</span></span>|<span data-ttu-id="7dd1d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dd1d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7dd1d-123">Accept</span></span>|<span data-ttu-id="7dd1d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7dd1d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dd1d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dd1d-125">Request body</span></span>
<span data-ttu-id="7dd1d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dd1d-127">响应</span><span class="sxs-lookup"><span data-stu-id="7dd1d-127">Response</span></span>
<span data-ttu-id="7dd1d-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-128">If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dd1d-129">示例</span><span class="sxs-lookup"><span data-stu-id="7dd1d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7dd1d-130">请求</span><span class="sxs-lookup"><span data-stu-id="7dd1d-130">Request</span></span>
<span data-ttu-id="7dd1d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7dd1d-132">响应</span><span class="sxs-lookup"><span data-stu-id="7dd1d-132">Response</span></span>
<span data-ttu-id="7dd1d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dd1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
      "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



