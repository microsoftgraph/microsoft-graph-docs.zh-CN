---
title: 获取 deviceComplianceScript
description: 读取 deviceComplianceScript 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b757611ac23a765734c75b0a8265ed009f2ba98
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128633"
---
# <a name="get-devicecompliancescript"></a><span data-ttu-id="623a0-103">获取 deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="623a0-103">Get deviceComplianceScript</span></span>

<span data-ttu-id="623a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="623a0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="623a0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="623a0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="623a0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="623a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="623a0-107">读取 [deviceComplianceScript 对象的属性和](../resources/intune-devices-devicecompliancescript.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="623a0-107">Read properties and relationships of the [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="623a0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="623a0-108">Prerequisites</span></span>
<span data-ttu-id="623a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="623a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="623a0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="623a0-111">Permission type</span></span>|<span data-ttu-id="623a0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="623a0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="623a0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="623a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="623a0-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623a0-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="623a0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="623a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="623a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="623a0-116">Not supported.</span></span>|
|<span data-ttu-id="623a0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="623a0-117">Application</span></span>|<span data-ttu-id="623a0-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623a0-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="623a0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="623a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="623a0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="623a0-120">Optional query parameters</span></span>
<span data-ttu-id="623a0-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="623a0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="623a0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="623a0-122">Request headers</span></span>
|<span data-ttu-id="623a0-123">标头</span><span class="sxs-lookup"><span data-stu-id="623a0-123">Header</span></span>|<span data-ttu-id="623a0-124">值</span><span class="sxs-lookup"><span data-stu-id="623a0-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="623a0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="623a0-125">Authorization</span></span>|<span data-ttu-id="623a0-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="623a0-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="623a0-127">接受</span><span class="sxs-lookup"><span data-stu-id="623a0-127">Accept</span></span>|<span data-ttu-id="623a0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="623a0-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="623a0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="623a0-129">Request body</span></span>
<span data-ttu-id="623a0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="623a0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="623a0-131">响应</span><span class="sxs-lookup"><span data-stu-id="623a0-131">Response</span></span>
<span data-ttu-id="623a0-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="623a0-132">If successful, this method returns a `200 OK` response code and [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="623a0-133">示例</span><span class="sxs-lookup"><span data-stu-id="623a0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="623a0-134">请求</span><span class="sxs-lookup"><span data-stu-id="623a0-134">Request</span></span>
<span data-ttu-id="623a0-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="623a0-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

### <a name="response"></a><span data-ttu-id="623a0-136">响应</span><span class="sxs-lookup"><span data-stu-id="623a0-136">Response</span></span>
<span data-ttu-id="623a0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="623a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 641

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScript",
    "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
    "publisher": "Publisher value",
    "version": "Version value",
    "displayName": "Display Name value",
    "description": "Description value",
    "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "runAsAccount": "user",
    "enforceSignatureCheck": true,
    "runAs32Bit": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




