---
title: importDeviceIdentityList 操作
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f0e00279f40d05e0162485d62a09b0b6827f25f7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423284"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="df423-103">importDeviceIdentityList 操作</span><span class="sxs-lookup"><span data-stu-id="df423-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="df423-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="df423-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df423-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df423-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df423-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df423-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df423-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df423-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df423-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df423-108">Prerequisites</span></span>
<span data-ttu-id="df423-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="df423-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df423-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df423-111">Permission type</span></span>|<span data-ttu-id="df423-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df423-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df423-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df423-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df423-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df423-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df423-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df423-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df423-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df423-116">Not supported.</span></span>|
|<span data-ttu-id="df423-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df423-117">Application</span></span>|<span data-ttu-id="df423-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="df423-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df423-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df423-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="df423-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df423-120">Request headers</span></span>
|<span data-ttu-id="df423-121">标头</span><span class="sxs-lookup"><span data-stu-id="df423-121">Header</span></span>|<span data-ttu-id="df423-122">值</span><span class="sxs-lookup"><span data-stu-id="df423-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df423-123">授权</span><span class="sxs-lookup"><span data-stu-id="df423-123">Authorization</span></span>|<span data-ttu-id="df423-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df423-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df423-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df423-125">Accept</span></span>|<span data-ttu-id="df423-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df423-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df423-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df423-127">Request body</span></span>
<span data-ttu-id="df423-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df423-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="df423-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="df423-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="df423-130">属性</span><span class="sxs-lookup"><span data-stu-id="df423-130">Property</span></span>|<span data-ttu-id="df423-131">类型</span><span class="sxs-lookup"><span data-stu-id="df423-131">Type</span></span>|<span data-ttu-id="df423-132">说明</span><span class="sxs-lookup"><span data-stu-id="df423-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df423-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="df423-133">importedDeviceIdentities</span></span>|<span data-ttu-id="df423-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)集合</span><span class="sxs-lookup"><span data-stu-id="df423-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="df423-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df423-135">Not yet documented</span></span>|
|<span data-ttu-id="df423-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="df423-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="df423-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="df423-137">Boolean</span></span>|<span data-ttu-id="df423-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df423-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="df423-139">响应</span><span class="sxs-lookup"><span data-stu-id="df423-139">Response</span></span>
<span data-ttu-id="df423-140">如果成功，此操作将返回`200 OK`响应代码和响应正文中的[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)集合。</span><span class="sxs-lookup"><span data-stu-id="df423-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df423-141">示例</span><span class="sxs-lookup"><span data-stu-id="df423-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="df423-142">请求</span><span class="sxs-lookup"><span data-stu-id="df423-142">Request</span></span>
<span data-ttu-id="df423-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df423-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="df423-144">响应</span><span class="sxs-lookup"><span data-stu-id="df423-144">Response</span></span>
<span data-ttu-id="df423-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df423-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




