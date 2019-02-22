---
title: 获取 iosLobAppProvisioningConfigurationAssignment
description: 读取 iosLobAppProvisioningConfigurationAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0ad6acfae1a180e5e3f66421525ee657e504a1c6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140724"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="fdeca-103">获取 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="fdeca-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="fdeca-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fdeca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdeca-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fdeca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdeca-106">读取[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fdeca-106">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdeca-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fdeca-107">Prerequisites</span></span>
<span data-ttu-id="fdeca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fdeca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fdeca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdeca-110">Permission type</span></span>|<span data-ttu-id="fdeca-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fdeca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdeca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdeca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdeca-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fdeca-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fdeca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdeca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdeca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdeca-115">Not supported.</span></span>|
|<span data-ttu-id="fdeca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdeca-116">Application</span></span>|<span data-ttu-id="fdeca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdeca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdeca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdeca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fdeca-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fdeca-119">Optional query parameters</span></span>
<span data-ttu-id="fdeca-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fdeca-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fdeca-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdeca-121">Request headers</span></span>
|<span data-ttu-id="fdeca-122">标头</span><span class="sxs-lookup"><span data-stu-id="fdeca-122">Header</span></span>|<span data-ttu-id="fdeca-123">值</span><span class="sxs-lookup"><span data-stu-id="fdeca-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdeca-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdeca-124">Authorization</span></span>|<span data-ttu-id="fdeca-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fdeca-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdeca-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fdeca-126">Accept</span></span>|<span data-ttu-id="fdeca-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fdeca-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdeca-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdeca-128">Request body</span></span>
<span data-ttu-id="fdeca-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdeca-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdeca-130">响应</span><span class="sxs-lookup"><span data-stu-id="fdeca-130">Response</span></span>
<span data-ttu-id="fdeca-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fdeca-131">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdeca-132">示例</span><span class="sxs-lookup"><span data-stu-id="fdeca-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdeca-133">请求</span><span class="sxs-lookup"><span data-stu-id="fdeca-133">Request</span></span>
<span data-ttu-id="fdeca-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fdeca-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="fdeca-135">响应</span><span class="sxs-lookup"><span data-stu-id="fdeca-135">Response</span></span>
<span data-ttu-id="fdeca-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fdeca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 262

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
    "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




