---
title: 列出 deviceHealthScripts
description: 列出 deviceHealthScript 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e80ad3290796b0f4fe5627255fc96f3cf199e918
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49225836"
---
# <a name="list-devicehealthscripts"></a><span data-ttu-id="6ab99-103">列出 deviceHealthScripts</span><span class="sxs-lookup"><span data-stu-id="6ab99-103">List deviceHealthScripts</span></span>

<span data-ttu-id="6ab99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ab99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ab99-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ab99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ab99-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ab99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ab99-107">列出 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6ab99-107">List properties and relationships of the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ab99-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6ab99-108">Prerequisites</span></span>
<span data-ttu-id="6ab99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ab99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab99-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ab99-111">Permission type</span></span>|<span data-ttu-id="6ab99-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6ab99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ab99-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ab99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ab99-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ab99-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6ab99-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ab99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ab99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ab99-116">Not supported.</span></span>|
|<span data-ttu-id="6ab99-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ab99-117">Application</span></span>|<span data-ttu-id="6ab99-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ab99-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ab99-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ab99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="6ab99-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ab99-120">Request headers</span></span>
|<span data-ttu-id="6ab99-121">标头</span><span class="sxs-lookup"><span data-stu-id="6ab99-121">Header</span></span>|<span data-ttu-id="6ab99-122">值</span><span class="sxs-lookup"><span data-stu-id="6ab99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ab99-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ab99-123">Authorization</span></span>|<span data-ttu-id="6ab99-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6ab99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ab99-125">接受</span><span class="sxs-lookup"><span data-stu-id="6ab99-125">Accept</span></span>|<span data-ttu-id="6ab99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ab99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ab99-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ab99-127">Request body</span></span>
<span data-ttu-id="6ab99-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ab99-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ab99-129">响应</span><span class="sxs-lookup"><span data-stu-id="6ab99-129">Response</span></span>
<span data-ttu-id="6ab99-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6ab99-130">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ab99-131">示例</span><span class="sxs-lookup"><span data-stu-id="6ab99-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ab99-132">请求</span><span class="sxs-lookup"><span data-stu-id="6ab99-132">Request</span></span>
<span data-ttu-id="6ab99-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ab99-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
```

### <a name="response"></a><span data-ttu-id="6ab99-134">响应</span><span class="sxs-lookup"><span data-stu-id="6ab99-134">Response</span></span>
<span data-ttu-id="6ab99-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ab99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1578

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScript",
      "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
      "publisher": "Publisher value",
      "version": "Version value",
      "displayName": "Display Name value",
      "description": "Description value",
      "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
      "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "runAsAccount": "user",
      "enforceSignatureCheck": true,
      "runAs32Bit": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "isGlobalScript": true,
      "highestAvailableVersion": "Highest Available Version value",
      "detectionScriptParameters": [
        {
          "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
          "name": "Name value",
          "description": "Description value",
          "isRequired": true,
          "applyDefaultValueWhenNotAssigned": true,
          "defaultValue": "Default Value value"
        }
      ],
      "remediationScriptParameters": [
        {
          "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
          "name": "Name value",
          "description": "Description value",
          "isRequired": true,
          "applyDefaultValueWhenNotAssigned": true,
          "defaultValue": "Default Value value"
        }
      ]
    }
  ]
}
```




