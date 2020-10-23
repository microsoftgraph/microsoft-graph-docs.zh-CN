---
title: 列出 enterpriseCodeSigningCertificates
description: 列出 enterpriseCodeSigningCertificate 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9e4ae90ec2c56ddc3abde81c310ae81cb2a49d8b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700456"
---
# <a name="list-enterprisecodesigningcertificates"></a><span data-ttu-id="ef403-103">列出 enterpriseCodeSigningCertificates</span><span class="sxs-lookup"><span data-stu-id="ef403-103">List enterpriseCodeSigningCertificates</span></span>

<span data-ttu-id="ef403-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef403-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ef403-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ef403-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef403-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ef403-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef403-107">列出 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ef403-107">List properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef403-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef403-108">Prerequisites</span></span>
<span data-ttu-id="ef403-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ef403-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef403-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef403-111">Permission type</span></span>|<span data-ttu-id="ef403-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef403-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef403-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef403-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef403-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef403-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ef403-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef403-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef403-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef403-116">Not supported.</span></span>|
|<span data-ttu-id="ef403-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef403-117">Application</span></span>|<span data-ttu-id="ef403-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ef403-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef403-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef403-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="ef403-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef403-120">Request headers</span></span>
|<span data-ttu-id="ef403-121">标头</span><span class="sxs-lookup"><span data-stu-id="ef403-121">Header</span></span>|<span data-ttu-id="ef403-122">值</span><span class="sxs-lookup"><span data-stu-id="ef403-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef403-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef403-123">Authorization</span></span>|<span data-ttu-id="ef403-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef403-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef403-125">接受</span><span class="sxs-lookup"><span data-stu-id="ef403-125">Accept</span></span>|<span data-ttu-id="ef403-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef403-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef403-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef403-127">Request body</span></span>
<span data-ttu-id="ef403-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ef403-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef403-129">响应</span><span class="sxs-lookup"><span data-stu-id="ef403-129">Response</span></span>
<span data-ttu-id="ef403-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ef403-130">If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef403-131">示例</span><span class="sxs-lookup"><span data-stu-id="ef403-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef403-132">请求</span><span class="sxs-lookup"><span data-stu-id="ef403-132">Request</span></span>
<span data-ttu-id="ef403-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef403-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### <a name="response"></a><span data-ttu-id="ef403-134">响应</span><span class="sxs-lookup"><span data-stu-id="ef403-134">Response</span></span>
<span data-ttu-id="ef403-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef403-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
      "id": "b20d3703-3703-b20d-0337-0db203370db2",
      "content": "Y29udGVudA==",
      "status": "provisioned",
      "subjectName": "Subject Name value",
      "subject": "Subject value",
      "issuerName": "Issuer Name value",
      "issuer": "Issuer value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
    }
  ]
}
```





