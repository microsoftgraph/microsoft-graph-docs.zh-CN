---
title: 获取 windows10EnterpriseModernAppManagementConfiguration
description: 读取 windows10EnterpriseModernAppManagementConfiguration 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a6d06cd83e400eca8591286c261e74f1569e4eaf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514068"
---
# <a name="get-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="d57ee-103">获取 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="d57ee-103">Get windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="d57ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d57ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d57ee-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d57ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d57ee-106">读取 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d57ee-106">Read properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d57ee-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d57ee-107">Prerequisites</span></span>
<span data-ttu-id="d57ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d57ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d57ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d57ee-110">Permission type</span></span>|<span data-ttu-id="d57ee-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d57ee-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d57ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d57ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d57ee-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d57ee-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d57ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d57ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d57ee-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d57ee-115">Not supported.</span></span>|
|<span data-ttu-id="d57ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d57ee-116">Application</span></span>|<span data-ttu-id="d57ee-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d57ee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d57ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d57ee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d57ee-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d57ee-119">Optional query parameters</span></span>
<span data-ttu-id="d57ee-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d57ee-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d57ee-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d57ee-121">Request headers</span></span>
|<span data-ttu-id="d57ee-122">标头</span><span class="sxs-lookup"><span data-stu-id="d57ee-122">Header</span></span>|<span data-ttu-id="d57ee-123">值</span><span class="sxs-lookup"><span data-stu-id="d57ee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d57ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d57ee-124">Authorization</span></span>|<span data-ttu-id="d57ee-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d57ee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d57ee-126">接受</span><span class="sxs-lookup"><span data-stu-id="d57ee-126">Accept</span></span>|<span data-ttu-id="d57ee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d57ee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d57ee-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d57ee-128">Request body</span></span>
<span data-ttu-id="d57ee-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d57ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d57ee-130">响应</span><span class="sxs-lookup"><span data-stu-id="d57ee-130">Response</span></span>
<span data-ttu-id="d57ee-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d57ee-131">If successful, this method returns a `200 OK` response code and [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d57ee-132">示例</span><span class="sxs-lookup"><span data-stu-id="d57ee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d57ee-133">请求</span><span class="sxs-lookup"><span data-stu-id="d57ee-133">Request</span></span>
<span data-ttu-id="d57ee-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d57ee-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d57ee-135">响应</span><span class="sxs-lookup"><span data-stu-id="d57ee-135">Response</span></span>
<span data-ttu-id="d57ee-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d57ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
    "id": "d6577687-7687-d657-8776-57d6877657d6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "uninstallBuiltInApps": true
  }
}
```




