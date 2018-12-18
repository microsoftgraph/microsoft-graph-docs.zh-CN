---
title: 列出 iosCertificateProfiles
description: 列出 iosCertificateProfile 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: cbf64ec3cccc2e972931c4c2598d02acbd4d57a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348396"
---
# <a name="list-ioscertificateprofiles"></a><span data-ttu-id="d87bf-103">列出 iosCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="d87bf-103">List iosCertificateProfiles</span></span>

> <span data-ttu-id="d87bf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d87bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d87bf-105">列出 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d87bf-105">List properties and relationships of the [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d87bf-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d87bf-106">Prerequisites</span></span>
<span data-ttu-id="d87bf-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d87bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d87bf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d87bf-109">Permission type</span></span>|<span data-ttu-id="d87bf-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d87bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d87bf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d87bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d87bf-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d87bf-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d87bf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d87bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d87bf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d87bf-114">Not supported.</span></span>|
|<span data-ttu-id="d87bf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d87bf-115">Application</span></span>|<span data-ttu-id="d87bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d87bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d87bf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d87bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d87bf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d87bf-118">Request headers</span></span>
|<span data-ttu-id="d87bf-119">标头</span><span class="sxs-lookup"><span data-stu-id="d87bf-119">Header</span></span>|<span data-ttu-id="d87bf-120">值</span><span class="sxs-lookup"><span data-stu-id="d87bf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d87bf-121">授权</span><span class="sxs-lookup"><span data-stu-id="d87bf-121">Authorization</span></span>|<span data-ttu-id="d87bf-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d87bf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d87bf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d87bf-123">Accept</span></span>|<span data-ttu-id="d87bf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d87bf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d87bf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d87bf-125">Request body</span></span>
<span data-ttu-id="d87bf-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d87bf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d87bf-127">响应</span><span class="sxs-lookup"><span data-stu-id="d87bf-127">Response</span></span>
<span data-ttu-id="d87bf-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d87bf-128">If successful, this method returns a `200 OK` response code and a collection of [iosCertificateProfile](../resources/intune-deviceconfig-ioscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d87bf-129">示例</span><span class="sxs-lookup"><span data-stu-id="d87bf-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d87bf-130">请求</span><span class="sxs-lookup"><span data-stu-id="d87bf-130">Request</span></span>
<span data-ttu-id="d87bf-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d87bf-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d87bf-132">响应</span><span class="sxs-lookup"><span data-stu-id="d87bf-132">Response</span></span>
<span data-ttu-id="d87bf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d87bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCertificateProfile",
      "id": "0ea4f39a-f39a-0ea4-9af3-a40e9af3a40e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```



