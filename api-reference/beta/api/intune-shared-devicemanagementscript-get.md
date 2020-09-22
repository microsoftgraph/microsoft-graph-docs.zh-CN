---
title: 获取 deviceManagementScript
description: 读取 deviceManagementScript 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 26d0c660d8285491fecbd7372a5018a6cf5d8d20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074326"
---
# <a name="get-devicemanagementscript"></a><span data-ttu-id="f7e92-103">获取 deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="f7e92-103">Get deviceManagementScript</span></span>

<span data-ttu-id="f7e92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7e92-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7e92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7e92-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7e92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7e92-107">读取 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7e92-107">Read properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7e92-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7e92-108">Prerequisites</span></span>
<span data-ttu-id="f7e92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7e92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7e92-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7e92-111">Permission type</span></span>|<span data-ttu-id="f7e92-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7e92-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7e92-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e92-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f7e92-114">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="f7e92-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f7e92-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7e92-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="f7e92-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="f7e92-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f7e92-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7e92-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="f7e92-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e92-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7e92-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7e92-119">Not supported.</span></span>|
|<span data-ttu-id="f7e92-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7e92-120">Application</span></span>||
| <span data-ttu-id="f7e92-121">&nbsp;&nbsp;**设备管理**</span><span class="sxs-lookup"><span data-stu-id="f7e92-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="f7e92-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7e92-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="f7e92-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="f7e92-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="f7e92-124">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7e92-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7e92-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7e92-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7e92-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f7e92-126">Optional query parameters</span></span>
<span data-ttu-id="f7e92-127">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f7e92-127">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7e92-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7e92-128">Request headers</span></span>
|<span data-ttu-id="f7e92-129">标头</span><span class="sxs-lookup"><span data-stu-id="f7e92-129">Header</span></span>|<span data-ttu-id="f7e92-130">值</span><span class="sxs-lookup"><span data-stu-id="f7e92-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7e92-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e92-131">Authorization</span></span>|<span data-ttu-id="f7e92-132">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7e92-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7e92-133">接受</span><span class="sxs-lookup"><span data-stu-id="f7e92-133">Accept</span></span>|<span data-ttu-id="f7e92-134">application/json</span><span class="sxs-lookup"><span data-stu-id="f7e92-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7e92-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7e92-135">Request body</span></span>
<span data-ttu-id="f7e92-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7e92-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e92-137">响应</span><span class="sxs-lookup"><span data-stu-id="f7e92-137">Response</span></span>
<span data-ttu-id="f7e92-138">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7e92-138">If successful, this method returns a `200 OK` response code and [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e92-139">示例</span><span class="sxs-lookup"><span data-stu-id="f7e92-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7e92-140">请求</span><span class="sxs-lookup"><span data-stu-id="f7e92-140">Request</span></span>
<span data-ttu-id="f7e92-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7e92-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

### <a name="response"></a><span data-ttu-id="f7e92-142">响应</span><span class="sxs-lookup"><span data-stu-id="f7e92-142">Response</span></span>
<span data-ttu-id="f7e92-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7e92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 668

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScript",
    "id": "59ea4525-4525-59ea-2545-ea592545ea59",
    "displayName": "Display Name value",
    "description": "Description value",
    "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
    },
    "scriptContent": "c2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "enforceSignatureCheck": true,
    "fileName": "File Name value",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "runAs32Bit": true
  }
}
```









