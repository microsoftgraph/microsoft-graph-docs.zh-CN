---
title: 列出 windows10EnterpriseModernAppManagementConfigurations
description: 列出 windows10EnterpriseModernAppManagementConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69506350a2b26525f038ca882967f6e71a705a42
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020204"
---
# <a name="list-windows10enterprisemodernappmanagementconfigurations"></a><span data-ttu-id="0f288-103">列出 windows10EnterpriseModernAppManagementConfigurations</span><span class="sxs-lookup"><span data-stu-id="0f288-103">List windows10EnterpriseModernAppManagementConfigurations</span></span>

> <span data-ttu-id="0f288-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f288-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f288-105">列出 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0f288-105">List properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f288-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="0f288-106">Prerequisites</span></span>
<span data-ttu-id="0f288-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0f288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f288-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0f288-109">Permission type</span></span>|<span data-ttu-id="0f288-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0f288-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f288-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0f288-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0f288-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0f288-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0f288-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0f288-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f288-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f288-114">Not supported.</span></span>|
|<span data-ttu-id="0f288-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0f288-115">Application</span></span>|<span data-ttu-id="0f288-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0f288-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f288-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0f288-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0f288-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0f288-118">Request headers</span></span>
|<span data-ttu-id="0f288-119">标头</span><span class="sxs-lookup"><span data-stu-id="0f288-119">Header</span></span>|<span data-ttu-id="0f288-120">值</span><span class="sxs-lookup"><span data-stu-id="0f288-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f288-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f288-121">Authorization</span></span>|<span data-ttu-id="0f288-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0f288-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f288-123">接受</span><span class="sxs-lookup"><span data-stu-id="0f288-123">Accept</span></span>|<span data-ttu-id="0f288-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0f288-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f288-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0f288-125">Request body</span></span>
<span data-ttu-id="0f288-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0f288-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0f288-127">响应</span><span class="sxs-lookup"><span data-stu-id="0f288-127">Response</span></span>
<span data-ttu-id="0f288-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0f288-128">If successful, this method returns a `200 OK` response code and a collection of [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f288-129">示例</span><span class="sxs-lookup"><span data-stu-id="0f288-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f288-130">请求</span><span class="sxs-lookup"><span data-stu-id="0f288-130">Request</span></span>
<span data-ttu-id="0f288-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0f288-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0f288-132">响应</span><span class="sxs-lookup"><span data-stu-id="0f288-132">Response</span></span>
<span data-ttu-id="0f288-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0f288-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
      "id": "d6577687-7687-d657-8776-57d6877657d6",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "uninstallBuiltInApps": true
    }
  ]
}
```



