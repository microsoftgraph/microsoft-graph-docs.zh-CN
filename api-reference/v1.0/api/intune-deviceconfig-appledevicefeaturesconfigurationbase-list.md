---
title: 列出 appleDeviceFeaturesConfigurationBases
description: 列出 appleDeviceFeaturesConfigurationBase 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 22ae72a38425c938fec8a1b2c4d9698c5355f6ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43400925"
---
# <a name="list-appledevicefeaturesconfigurationbases"></a><span data-ttu-id="71674-103">列出 appleDeviceFeaturesConfigurationBases</span><span class="sxs-lookup"><span data-stu-id="71674-103">List appleDeviceFeaturesConfigurationBases</span></span>

<span data-ttu-id="71674-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71674-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71674-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71674-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71674-106">列出 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71674-106">List properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71674-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="71674-107">Prerequisites</span></span>
<span data-ttu-id="71674-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71674-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="71674-110">Permission type</span></span>|<span data-ttu-id="71674-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71674-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71674-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71674-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71674-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="71674-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="71674-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71674-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71674-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="71674-115">Not supported.</span></span>|
|<span data-ttu-id="71674-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="71674-116">Application</span></span>|<span data-ttu-id="71674-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="71674-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71674-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71674-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71674-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="71674-119">Request headers</span></span>
|<span data-ttu-id="71674-120">标头</span><span class="sxs-lookup"><span data-stu-id="71674-120">Header</span></span>|<span data-ttu-id="71674-121">值</span><span class="sxs-lookup"><span data-stu-id="71674-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71674-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71674-122">Authorization</span></span>|<span data-ttu-id="71674-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71674-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71674-124">接受</span><span class="sxs-lookup"><span data-stu-id="71674-124">Accept</span></span>|<span data-ttu-id="71674-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71674-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71674-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71674-126">Request body</span></span>
<span data-ttu-id="71674-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71674-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71674-128">响应</span><span class="sxs-lookup"><span data-stu-id="71674-128">Response</span></span>
<span data-ttu-id="71674-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="71674-129">If successful, this method returns a `200 OK` response code and a collection of [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71674-130">示例</span><span class="sxs-lookup"><span data-stu-id="71674-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="71674-131">请求</span><span class="sxs-lookup"><span data-stu-id="71674-131">Request</span></span>
<span data-ttu-id="71674-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71674-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="71674-133">响应</span><span class="sxs-lookup"><span data-stu-id="71674-133">Response</span></span>
<span data-ttu-id="71674-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71674-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






