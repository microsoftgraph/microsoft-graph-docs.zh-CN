---
title: 获取 iosLobAppProvisioningConfigurationAssignment
description: 读取 iosLobAppProvisioningConfigurationAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a930d78ee8e234fc6a548af86c9057360724362d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793393"
---
# <a name="get-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="ed545-103">获取 iosLobAppProvisioningConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ed545-103">Get iosLobAppProvisioningConfigurationAssignment</span></span>

<span data-ttu-id="ed545-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed545-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed545-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ed545-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed545-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed545-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed545-107">读取[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed545-107">Read properties and relationships of the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed545-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ed545-108">Prerequisites</span></span>
<span data-ttu-id="ed545-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="ed545-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ed545-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed545-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed545-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed545-111">Permission type</span></span>|<span data-ttu-id="ed545-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ed545-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed545-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed545-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ed545-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed545-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ed545-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed545-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed545-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed545-116">Not supported.</span></span>|
|<span data-ttu-id="ed545-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed545-117">Application</span></span>|<span data-ttu-id="ed545-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed545-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed545-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed545-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed545-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed545-120">Optional query parameters</span></span>
<span data-ttu-id="ed545-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed545-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed545-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed545-122">Request headers</span></span>
|<span data-ttu-id="ed545-123">标头</span><span class="sxs-lookup"><span data-stu-id="ed545-123">Header</span></span>|<span data-ttu-id="ed545-124">值</span><span class="sxs-lookup"><span data-stu-id="ed545-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed545-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed545-125">Authorization</span></span>|<span data-ttu-id="ed545-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ed545-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed545-127">接受</span><span class="sxs-lookup"><span data-stu-id="ed545-127">Accept</span></span>|<span data-ttu-id="ed545-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ed545-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed545-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed545-129">Request body</span></span>
<span data-ttu-id="ed545-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed545-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed545-131">响应</span><span class="sxs-lookup"><span data-stu-id="ed545-131">Response</span></span>
<span data-ttu-id="ed545-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ed545-132">If successful, this method returns a `200 OK` response code and [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed545-133">示例</span><span class="sxs-lookup"><span data-stu-id="ed545-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed545-134">请求</span><span class="sxs-lookup"><span data-stu-id="ed545-134">Request</span></span>
<span data-ttu-id="ed545-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ed545-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ed545-136">响应</span><span class="sxs-lookup"><span data-stu-id="ed545-136">Response</span></span>
<span data-ttu-id="ed545-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="ed545-137">Here is an example of the response.</span></span> <span data-ttu-id="ed545-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="ed545-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ed545-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="ed545-139">All of the properties will be returned from an actual call.</span></span>
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



