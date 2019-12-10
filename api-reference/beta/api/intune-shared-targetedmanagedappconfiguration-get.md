---
title: 获取 targetedManagedAppConfiguration
description: 读取 targetedManagedAppConfiguration 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 27d275f1cb310d4ab6a82ce394bbd13389ea7917
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939541"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="a4ca2-103">获取 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a4ca2-103">Get targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="a4ca2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4ca2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4ca2-106">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-106">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4ca2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a4ca2-107">Prerequisites</span></span>
<span data-ttu-id="a4ca2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4ca2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4ca2-110">Permission type</span></span>|<span data-ttu-id="a4ca2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a4ca2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4ca2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4ca2-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a4ca2-113">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a4ca2-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="a4ca2-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4ca2-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="a4ca2-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="a4ca2-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a4ca2-116">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4ca2-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a4ca2-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4ca2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4ca2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-118">Not supported.</span></span>|
|<span data-ttu-id="a4ca2-119">Application</span><span class="sxs-lookup"><span data-stu-id="a4ca2-119">Application</span></span>||
| <span data-ttu-id="a4ca2-120">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="a4ca2-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="a4ca2-121">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4ca2-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="a4ca2-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="a4ca2-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="a4ca2-123">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4ca2-123">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4ca2-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4ca2-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a4ca2-125">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4ca2-125">Optional query parameters</span></span>
<span data-ttu-id="a4ca2-126">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-126">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4ca2-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4ca2-127">Request headers</span></span>
|<span data-ttu-id="a4ca2-128">标头</span><span class="sxs-lookup"><span data-stu-id="a4ca2-128">Header</span></span>|<span data-ttu-id="a4ca2-129">值</span><span class="sxs-lookup"><span data-stu-id="a4ca2-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4ca2-130">授权</span><span class="sxs-lookup"><span data-stu-id="a4ca2-130">Authorization</span></span>|<span data-ttu-id="a4ca2-131">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4ca2-132">接受</span><span class="sxs-lookup"><span data-stu-id="a4ca2-132">Accept</span></span>|<span data-ttu-id="a4ca2-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a4ca2-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4ca2-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4ca2-134">Request body</span></span>
<span data-ttu-id="a4ca2-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4ca2-136">响应</span><span class="sxs-lookup"><span data-stu-id="a4ca2-136">Response</span></span>
<span data-ttu-id="a4ca2-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-137">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4ca2-138">示例</span><span class="sxs-lookup"><span data-stu-id="a4ca2-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4ca2-139">请求</span><span class="sxs-lookup"><span data-stu-id="a4ca2-139">Request</span></span>
<span data-ttu-id="a4ca2-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a4ca2-141">响应</span><span class="sxs-lookup"><span data-stu-id="a4ca2-141">Response</span></span>
<span data-ttu-id="a4ca2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4ca2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "2444e029-e029-2444-29e0-442429e04424",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "deployedAppCount": 0,
    "isAssigned": true
  }
}
```








