---
title: 列出 androidDeviceOwnerEnrollmentProfiles
description: 列出 androidDeviceOwnerEnrollmentProfile 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74cb5100feb61e76103e448a20b88c8953a51fc6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705210"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="c37a2-103">列出 androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="c37a2-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="c37a2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c37a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c37a2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c37a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c37a2-106">列出[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c37a2-106">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c37a2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c37a2-107">Prerequisites</span></span>
<span data-ttu-id="c37a2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c37a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c37a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c37a2-110">Permission type</span></span>|<span data-ttu-id="c37a2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c37a2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c37a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c37a2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c37a2-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c37a2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c37a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c37a2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c37a2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c37a2-115">Not supported.</span></span>|
|<span data-ttu-id="c37a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c37a2-116">Application</span></span>|<span data-ttu-id="c37a2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c37a2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c37a2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c37a2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c37a2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c37a2-119">Request headers</span></span>
|<span data-ttu-id="c37a2-120">标头</span><span class="sxs-lookup"><span data-stu-id="c37a2-120">Header</span></span>|<span data-ttu-id="c37a2-121">值</span><span class="sxs-lookup"><span data-stu-id="c37a2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c37a2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c37a2-122">Authorization</span></span>|<span data-ttu-id="c37a2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c37a2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c37a2-124">接受</span><span class="sxs-lookup"><span data-stu-id="c37a2-124">Accept</span></span>|<span data-ttu-id="c37a2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c37a2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c37a2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c37a2-126">Request body</span></span>
<span data-ttu-id="c37a2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c37a2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c37a2-128">响应</span><span class="sxs-lookup"><span data-stu-id="c37a2-128">Response</span></span>
<span data-ttu-id="c37a2-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c37a2-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c37a2-130">示例</span><span class="sxs-lookup"><span data-stu-id="c37a2-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c37a2-131">请求</span><span class="sxs-lookup"><span data-stu-id="c37a2-131">Request</span></span>
<span data-ttu-id="c37a2-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c37a2-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="c37a2-133">响应</span><span class="sxs-lookup"><span data-stu-id="c37a2-133">Response</span></span>
<span data-ttu-id="c37a2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c37a2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 898

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
      "accountId": "Account Id value",
      "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "tokenValue": "Token Value value",
      "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
      "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
      "enrolledDeviceCount": 3,
      "qrCodeContent": "Qr Code Content value",
      "qrCodeImage": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "scopeTags": [
        "Scope Tags value"
      ]
    }
  ]
}
```





