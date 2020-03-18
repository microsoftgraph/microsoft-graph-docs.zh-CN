---
title: 列出 securityBaselineDeviceStates
description: 列出 securityBaselineDeviceState 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a58e76054e5485b90ff963faedf93f63d50e383
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764500"
---
# <a name="list-securitybaselinedevicestates"></a><span data-ttu-id="c75db-103">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="c75db-103">List securityBaselineDeviceStates</span></span>

> <span data-ttu-id="c75db-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c75db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c75db-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c75db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c75db-106">列出[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c75db-106">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c75db-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c75db-107">Prerequisites</span></span>
<span data-ttu-id="c75db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c75db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c75db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c75db-110">Permission type</span></span>|<span data-ttu-id="c75db-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c75db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c75db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c75db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c75db-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c75db-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c75db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c75db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c75db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c75db-115">Not supported.</span></span>|
|<span data-ttu-id="c75db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c75db-116">Application</span></span>|<span data-ttu-id="c75db-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c75db-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c75db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c75db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="c75db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c75db-119">Request headers</span></span>
|<span data-ttu-id="c75db-120">标头</span><span class="sxs-lookup"><span data-stu-id="c75db-120">Header</span></span>|<span data-ttu-id="c75db-121">值</span><span class="sxs-lookup"><span data-stu-id="c75db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c75db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c75db-122">Authorization</span></span>|<span data-ttu-id="c75db-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c75db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c75db-124">接受</span><span class="sxs-lookup"><span data-stu-id="c75db-124">Accept</span></span>|<span data-ttu-id="c75db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c75db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c75db-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c75db-126">Request body</span></span>
<span data-ttu-id="c75db-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c75db-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c75db-128">响应</span><span class="sxs-lookup"><span data-stu-id="c75db-128">Response</span></span>
<span data-ttu-id="c75db-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c75db-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c75db-130">示例</span><span class="sxs-lookup"><span data-stu-id="c75db-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c75db-131">请求</span><span class="sxs-lookup"><span data-stu-id="c75db-131">Request</span></span>
<span data-ttu-id="c75db-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c75db-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

### <a name="response"></a><span data-ttu-id="c75db-133">响应</span><span class="sxs-lookup"><span data-stu-id="c75db-133">Response</span></span>
<span data-ttu-id="c75db-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c75db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
      "id": "182749bf-49bf-1827-bf49-2718bf492718",
      "managedDeviceId": "Managed Device Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "state": "secure",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
    }
  ]
}
```




