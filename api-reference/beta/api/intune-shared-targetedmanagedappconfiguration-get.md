---
title: 获取 targetedManagedAppConfiguration
description: 读取 targetedManagedAppConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 072236e623bc70c6b3ba132d148a71adbacdbabf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217470"
---
# <a name="get-targetedmanagedappconfiguration"></a><span data-ttu-id="264ed-103">获取 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="264ed-103">Get targetedManagedAppConfiguration</span></span>

<span data-ttu-id="264ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="264ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="264ed-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="264ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="264ed-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="264ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="264ed-107">读取 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="264ed-107">Read properties and relationships of the [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="264ed-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="264ed-108">Prerequisites</span></span>
<span data-ttu-id="264ed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="264ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="264ed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="264ed-111">Permission type</span></span>|<span data-ttu-id="264ed-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="264ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="264ed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="264ed-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="264ed-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="264ed-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="264ed-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="264ed-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="264ed-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="264ed-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="264ed-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="264ed-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="264ed-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="264ed-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="264ed-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="264ed-119">Not supported.</span></span>|
|<span data-ttu-id="264ed-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="264ed-120">Application</span></span>||
| <span data-ttu-id="264ed-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="264ed-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="264ed-122">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="264ed-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="264ed-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="264ed-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="264ed-124">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="264ed-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="264ed-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="264ed-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="264ed-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="264ed-126">Optional query parameters</span></span>
<span data-ttu-id="264ed-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="264ed-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="264ed-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="264ed-128">Request headers</span></span>
|<span data-ttu-id="264ed-129">标头</span><span class="sxs-lookup"><span data-stu-id="264ed-129">Header</span></span>|<span data-ttu-id="264ed-130">值</span><span class="sxs-lookup"><span data-stu-id="264ed-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="264ed-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="264ed-131">Authorization</span></span>|<span data-ttu-id="264ed-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="264ed-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="264ed-133">接受</span><span class="sxs-lookup"><span data-stu-id="264ed-133">Accept</span></span>|<span data-ttu-id="264ed-134">application/json</span><span class="sxs-lookup"><span data-stu-id="264ed-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="264ed-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="264ed-135">Request body</span></span>
<span data-ttu-id="264ed-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="264ed-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="264ed-137">响应</span><span class="sxs-lookup"><span data-stu-id="264ed-137">Response</span></span>
<span data-ttu-id="264ed-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="264ed-138">If successful, this method returns a `200 OK` response code and [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="264ed-139">示例</span><span class="sxs-lookup"><span data-stu-id="264ed-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="264ed-140">请求</span><span class="sxs-lookup"><span data-stu-id="264ed-140">Request</span></span>
<span data-ttu-id="264ed-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="264ed-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="264ed-142">响应</span><span class="sxs-lookup"><span data-stu-id="264ed-142">Response</span></span>
<span data-ttu-id="264ed-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="264ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







