---
title: 列出 deviceManagementScripts
description: 列出 deviceManagementScript 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 056f8c012ba31322f0afcc824f3fab67fe681c65
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867747"
---
# <a name="list-devicemanagementscripts"></a><span data-ttu-id="6ce15-103">列出 deviceManagementScripts</span><span class="sxs-lookup"><span data-stu-id="6ce15-103">List deviceManagementScripts</span></span>

<span data-ttu-id="6ce15-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ce15-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ce15-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ce15-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ce15-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ce15-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ce15-107">列出 [deviceManagementScript 对象的属性和](../resources/intune-shared-devicemanagementscript.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="6ce15-107">List properties and relationships of the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ce15-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ce15-108">Prerequisites</span></span>
<span data-ttu-id="6ce15-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ce15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ce15-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ce15-111">Permission type</span></span>|<span data-ttu-id="6ce15-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6ce15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ce15-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ce15-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6ce15-114">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6ce15-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6ce15-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ce15-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6ce15-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="6ce15-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6ce15-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ce15-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6ce15-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ce15-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ce15-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ce15-119">Not supported.</span></span>|
|<span data-ttu-id="6ce15-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ce15-120">Application</span></span>||
| <span data-ttu-id="6ce15-121">&nbsp; &nbsp; **设备管理**</span><span class="sxs-lookup"><span data-stu-id="6ce15-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6ce15-122">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ce15-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6ce15-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="6ce15-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6ce15-124">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ce15-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ce15-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ce15-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="6ce15-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ce15-126">Request headers</span></span>
|<span data-ttu-id="6ce15-127">标头</span><span class="sxs-lookup"><span data-stu-id="6ce15-127">Header</span></span>|<span data-ttu-id="6ce15-128">值</span><span class="sxs-lookup"><span data-stu-id="6ce15-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ce15-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ce15-129">Authorization</span></span>|<span data-ttu-id="6ce15-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ce15-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ce15-131">接受</span><span class="sxs-lookup"><span data-stu-id="6ce15-131">Accept</span></span>|<span data-ttu-id="6ce15-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6ce15-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ce15-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ce15-133">Request body</span></span>
<span data-ttu-id="6ce15-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ce15-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ce15-135">响应</span><span class="sxs-lookup"><span data-stu-id="6ce15-135">Response</span></span>
<span data-ttu-id="6ce15-136">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6ce15-136">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ce15-137">示例</span><span class="sxs-lookup"><span data-stu-id="6ce15-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ce15-138">请求</span><span class="sxs-lookup"><span data-stu-id="6ce15-138">Request</span></span>
<span data-ttu-id="6ce15-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ce15-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
```

### <a name="response"></a><span data-ttu-id="6ce15-140">响应</span><span class="sxs-lookup"><span data-stu-id="6ce15-140">Response</span></span>
<span data-ttu-id="6ce15-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ce15-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
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
  ]
}
```







