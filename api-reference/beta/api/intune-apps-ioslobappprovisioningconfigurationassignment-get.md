---
title: 获取 iosLobAppProvisioningConfigurationAssignment
description: 读取 iosLobAppProvisioningConfigurationAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b2aa3dfe193e19c3cdb67985d7eaabfb22fd849
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144233"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="3909d-103">获取 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="3909d-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="3909d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3909d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3909d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3909d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3909d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3909d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3909d-107">读取 [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3909d-107">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3909d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3909d-108">Prerequisites</span></span>
<span data-ttu-id="3909d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3909d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3909d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3909d-111">Permission type</span></span>|<span data-ttu-id="3909d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3909d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3909d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3909d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3909d-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3909d-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3909d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3909d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3909d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3909d-116">Not supported.</span></span>|
|<span data-ttu-id="3909d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3909d-117">Application</span></span>|<span data-ttu-id="3909d-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3909d-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3909d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3909d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3909d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3909d-120">Optional query parameters</span></span>
<span data-ttu-id="3909d-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3909d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3909d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3909d-122">Request headers</span></span>
|<span data-ttu-id="3909d-123">标头</span><span class="sxs-lookup"><span data-stu-id="3909d-123">Header</span></span>|<span data-ttu-id="3909d-124">值</span><span class="sxs-lookup"><span data-stu-id="3909d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3909d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3909d-125">Authorization</span></span>|<span data-ttu-id="3909d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3909d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3909d-127">接受</span><span class="sxs-lookup"><span data-stu-id="3909d-127">Accept</span></span>|<span data-ttu-id="3909d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3909d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3909d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3909d-129">Request body</span></span>
<span data-ttu-id="3909d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3909d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3909d-131">响应</span><span class="sxs-lookup"><span data-stu-id="3909d-131">Response</span></span>
<span data-ttu-id="3909d-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3909d-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3909d-133">示例</span><span class="sxs-lookup"><span data-stu-id="3909d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3909d-134">请求</span><span class="sxs-lookup"><span data-stu-id="3909d-134">Request</span></span>
<span data-ttu-id="3909d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3909d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="3909d-136">响应</span><span class="sxs-lookup"><span data-stu-id="3909d-136">Response</span></span>
<span data-ttu-id="3909d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3909d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 433

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
    "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    }
  }
}
```




