---
title: importDeviceIdentityList 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c41b74df62ab444b86ad3c8e2f009413d94aa94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466624"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="b1837-103">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="b1837-103">importDeviceIdentityList action</span></span>

<span data-ttu-id="b1837-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b1837-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1837-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1837-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1837-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1837-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1837-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1837-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1837-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1837-108">Prerequisites</span></span>
<span data-ttu-id="b1837-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1837-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1837-111">Permission type</span></span>|<span data-ttu-id="b1837-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1837-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1837-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1837-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1837-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1837-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b1837-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1837-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1837-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1837-116">Not supported.</span></span>|
|<span data-ttu-id="b1837-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1837-117">Application</span></span>|<span data-ttu-id="b1837-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1837-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1837-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1837-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="b1837-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1837-120">Request headers</span></span>
|<span data-ttu-id="b1837-121">标头</span><span class="sxs-lookup"><span data-stu-id="b1837-121">Header</span></span>|<span data-ttu-id="b1837-122">值</span><span class="sxs-lookup"><span data-stu-id="b1837-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1837-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1837-123">Authorization</span></span>|<span data-ttu-id="b1837-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1837-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1837-125">接受</span><span class="sxs-lookup"><span data-stu-id="b1837-125">Accept</span></span>|<span data-ttu-id="b1837-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1837-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1837-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1837-127">Request body</span></span>
<span data-ttu-id="b1837-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1837-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b1837-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="b1837-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b1837-130">属性</span><span class="sxs-lookup"><span data-stu-id="b1837-130">Property</span></span>|<span data-ttu-id="b1837-131">类型</span><span class="sxs-lookup"><span data-stu-id="b1837-131">Type</span></span>|<span data-ttu-id="b1837-132">说明</span><span class="sxs-lookup"><span data-stu-id="b1837-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1837-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="b1837-133">importedDeviceIdentities</span></span>|<span data-ttu-id="b1837-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="b1837-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="b1837-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1837-135">Not yet documented</span></span>|
|<span data-ttu-id="b1837-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="b1837-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="b1837-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1837-137">Boolean</span></span>|<span data-ttu-id="b1837-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b1837-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1837-139">响应</span><span class="sxs-lookup"><span data-stu-id="b1837-139">Response</span></span>
<span data-ttu-id="b1837-140">如果成功，此操作会在`200 OK`响应正文中返回响应代码和[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="b1837-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1837-141">示例</span><span class="sxs-lookup"><span data-stu-id="b1837-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1837-142">请求</span><span class="sxs-lookup"><span data-stu-id="b1837-142">Request</span></span>
<span data-ttu-id="b1837-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1837-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="b1837-144">响应</span><span class="sxs-lookup"><span data-stu-id="b1837-144">Response</span></span>
<span data-ttu-id="b1837-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1837-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```





