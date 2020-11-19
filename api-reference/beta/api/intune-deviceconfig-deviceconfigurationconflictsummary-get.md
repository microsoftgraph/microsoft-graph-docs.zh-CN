---
title: 获取 deviceConfigurationConflictSummary
description: 读取 deviceConfigurationConflictSummary 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6c2bffcd19b7a5527e2a0a775c4a30b29ec6ac33
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291755"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="91e9d-103">获取 deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="91e9d-103">Get deviceConfigurationConflictSummary</span></span>

<span data-ttu-id="91e9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91e9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91e9d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="91e9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91e9d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="91e9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91e9d-107">读取 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="91e9d-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91e9d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="91e9d-108">Prerequisites</span></span>
<span data-ttu-id="91e9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91e9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91e9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="91e9d-111">Permission type</span></span>|<span data-ttu-id="91e9d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="91e9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91e9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91e9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91e9d-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="91e9d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="91e9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91e9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91e9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="91e9d-116">Not supported.</span></span>|
|<span data-ttu-id="91e9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="91e9d-117">Application</span></span>|<span data-ttu-id="91e9d-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="91e9d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91e9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91e9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91e9d-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="91e9d-120">Optional query parameters</span></span>
<span data-ttu-id="91e9d-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="91e9d-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91e9d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="91e9d-122">Request headers</span></span>
|<span data-ttu-id="91e9d-123">标头</span><span class="sxs-lookup"><span data-stu-id="91e9d-123">Header</span></span>|<span data-ttu-id="91e9d-124">值</span><span class="sxs-lookup"><span data-stu-id="91e9d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91e9d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="91e9d-125">Authorization</span></span>|<span data-ttu-id="91e9d-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="91e9d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91e9d-127">接受</span><span class="sxs-lookup"><span data-stu-id="91e9d-127">Accept</span></span>|<span data-ttu-id="91e9d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="91e9d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91e9d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="91e9d-129">Request body</span></span>
<span data-ttu-id="91e9d-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="91e9d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91e9d-131">响应</span><span class="sxs-lookup"><span data-stu-id="91e9d-131">Response</span></span>
<span data-ttu-id="91e9d-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91e9d-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91e9d-133">示例</span><span class="sxs-lookup"><span data-stu-id="91e9d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="91e9d-134">请求</span><span class="sxs-lookup"><span data-stu-id="91e9d-134">Request</span></span>
<span data-ttu-id="91e9d-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91e9d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="91e9d-136">响应</span><span class="sxs-lookup"><span data-stu-id="91e9d-136">Response</span></span>
<span data-ttu-id="91e9d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91e9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value",
        "sourceType": "deviceIntent"
      }
    ],
    "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
    "contributingSettings": [
      "Contributing Settings value"
    ],
    "deviceCheckinsImpacted": 6
  }
}
```




