---
title: 获取 androidDeviceOwnerEnrollmentProfile
description: 读取属性和 androidDeviceOwnerEnrollmentProfile 对象的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b6aa495abc2bb5bd72583a01112292fa9c476f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406498"
---
# <a name="get-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="a7562-103">获取 androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a7562-103">Get androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="a7562-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a7562-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7562-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7562-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7562-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7562-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7562-107">读取属性和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="a7562-107">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7562-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7562-108">Prerequisites</span></span>
<span data-ttu-id="a7562-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a7562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7562-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7562-111">Permission type</span></span>|<span data-ttu-id="a7562-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7562-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7562-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7562-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7562-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7562-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a7562-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7562-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7562-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7562-116">Not supported.</span></span>|
|<span data-ttu-id="a7562-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7562-117">Application</span></span>|<span data-ttu-id="a7562-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7562-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7562-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7562-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7562-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7562-120">Optional query parameters</span></span>
<span data-ttu-id="a7562-121">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7562-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7562-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7562-122">Request headers</span></span>
|<span data-ttu-id="a7562-123">标头</span><span class="sxs-lookup"><span data-stu-id="a7562-123">Header</span></span>|<span data-ttu-id="a7562-124">值</span><span class="sxs-lookup"><span data-stu-id="a7562-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7562-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7562-125">Authorization</span></span>|<span data-ttu-id="a7562-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7562-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7562-127">Accept</span><span class="sxs-lookup"><span data-stu-id="a7562-127">Accept</span></span>|<span data-ttu-id="a7562-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a7562-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7562-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7562-129">Request body</span></span>
<span data-ttu-id="a7562-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7562-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7562-131">响应</span><span class="sxs-lookup"><span data-stu-id="a7562-131">Response</span></span>
<span data-ttu-id="a7562-132">如果成功，此方法返回`200 OK`响应正文中的响应代码和[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a7562-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7562-133">示例</span><span class="sxs-lookup"><span data-stu-id="a7562-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7562-134">请求</span><span class="sxs-lookup"><span data-stu-id="a7562-134">Request</span></span>
<span data-ttu-id="a7562-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7562-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="a7562-136">响应</span><span class="sxs-lookup"><span data-stu-id="a7562-136">Response</span></span>
<span data-ttu-id="a7562-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7562-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

{
  "value": {
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
    }
  }
}
```




