---
title: 列出 importedDeviceIdentities
description: 列出 importedDeviceIdentity 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 085fcb716930ecaa303933aa2119a6b73b83680e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985068"
---
# <a name="list-importeddeviceidentities"></a><span data-ttu-id="4c106-103">列出 importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="4c106-103">List importedDeviceIdentities</span></span>

> <span data-ttu-id="4c106-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4c106-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c106-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c106-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c106-106">列出[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c106-106">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c106-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c106-107">Prerequisites</span></span>
<span data-ttu-id="4c106-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c106-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c106-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c106-110">Permission type</span></span>|<span data-ttu-id="4c106-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c106-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c106-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c106-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c106-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c106-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="4c106-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c106-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c106-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c106-115">Not supported.</span></span>|
|<span data-ttu-id="4c106-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c106-116">Application</span></span>|<span data-ttu-id="4c106-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c106-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c106-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c106-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="4c106-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c106-119">Request headers</span></span>
|<span data-ttu-id="4c106-120">标头</span><span class="sxs-lookup"><span data-stu-id="4c106-120">Header</span></span>|<span data-ttu-id="4c106-121">值</span><span class="sxs-lookup"><span data-stu-id="4c106-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c106-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c106-122">Authorization</span></span>|<span data-ttu-id="4c106-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c106-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c106-124">接受</span><span class="sxs-lookup"><span data-stu-id="4c106-124">Accept</span></span>|<span data-ttu-id="4c106-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c106-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c106-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c106-126">Request body</span></span>
<span data-ttu-id="4c106-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4c106-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c106-128">响应</span><span class="sxs-lookup"><span data-stu-id="4c106-128">Response</span></span>
<span data-ttu-id="4c106-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4c106-129">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c106-130">示例</span><span class="sxs-lookup"><span data-stu-id="4c106-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c106-131">请求</span><span class="sxs-lookup"><span data-stu-id="4c106-131">Request</span></span>
<span data-ttu-id="4c106-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c106-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="4c106-133">响应</span><span class="sxs-lookup"><span data-stu-id="4c106-133">Response</span></span>
<span data-ttu-id="4c106-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c106-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
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
  ]
}
```





