---
title: 列出 mobileAppProvisioningConfigGroupAssignments
description: 列出 mobileAppProvisioningConfigGroupAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eee41c794fe96169a81395f2126cbba3ba467091
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935046"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="db167-103">列出 mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="db167-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="db167-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="db167-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db167-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="db167-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db167-106">列出[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db167-106">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db167-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="db167-107">Prerequisites</span></span>
<span data-ttu-id="db167-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db167-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db167-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="db167-110">Permission type</span></span>|<span data-ttu-id="db167-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db167-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db167-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db167-112">Delegated (work or school account)</span></span>|<span data-ttu-id="db167-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="db167-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="db167-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db167-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db167-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="db167-115">Not supported.</span></span>|
|<span data-ttu-id="db167-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="db167-116">Application</span></span>|<span data-ttu-id="db167-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="db167-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db167-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db167-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="db167-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="db167-119">Request headers</span></span>
|<span data-ttu-id="db167-120">标头</span><span class="sxs-lookup"><span data-stu-id="db167-120">Header</span></span>|<span data-ttu-id="db167-121">值</span><span class="sxs-lookup"><span data-stu-id="db167-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db167-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="db167-122">Authorization</span></span>|<span data-ttu-id="db167-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db167-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db167-124">接受</span><span class="sxs-lookup"><span data-stu-id="db167-124">Accept</span></span>|<span data-ttu-id="db167-125">application/json</span><span class="sxs-lookup"><span data-stu-id="db167-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db167-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="db167-126">Request body</span></span>
<span data-ttu-id="db167-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db167-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db167-128">响应</span><span class="sxs-lookup"><span data-stu-id="db167-128">Response</span></span>
<span data-ttu-id="db167-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="db167-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db167-130">示例</span><span class="sxs-lookup"><span data-stu-id="db167-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="db167-131">请求</span><span class="sxs-lookup"><span data-stu-id="db167-131">Request</span></span>
<span data-ttu-id="db167-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db167-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="db167-133">响应</span><span class="sxs-lookup"><span data-stu-id="db167-133">Response</span></span>
<span data-ttu-id="db167-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db167-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ]
}
```




