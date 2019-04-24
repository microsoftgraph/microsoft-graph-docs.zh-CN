---
title: 获取 symantecCodeSigningCertificate
description: 读取 symantecCodeSigningCertificate 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 396821b7e5250347ebec2d8bb28a52312b58c93d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32488748"
---
# <a name="get-symanteccodesigningcertificate"></a><span data-ttu-id="4aaff-103">获取 symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="4aaff-103">Get symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="4aaff-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4aaff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4aaff-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4aaff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aaff-106">读取[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4aaff-106">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4aaff-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4aaff-107">Prerequisites</span></span>
<span data-ttu-id="4aaff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aaff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aaff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aaff-110">Permission type</span></span>|<span data-ttu-id="4aaff-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4aaff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4aaff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aaff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4aaff-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4aaff-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4aaff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aaff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aaff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4aaff-115">Not supported.</span></span>|
|<span data-ttu-id="4aaff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aaff-116">Application</span></span>|<span data-ttu-id="4aaff-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4aaff-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4aaff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aaff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4aaff-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4aaff-119">Optional query parameters</span></span>
<span data-ttu-id="4aaff-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4aaff-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4aaff-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aaff-121">Request headers</span></span>
|<span data-ttu-id="4aaff-122">标头</span><span class="sxs-lookup"><span data-stu-id="4aaff-122">Header</span></span>|<span data-ttu-id="4aaff-123">值</span><span class="sxs-lookup"><span data-stu-id="4aaff-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4aaff-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aaff-124">Authorization</span></span>|<span data-ttu-id="4aaff-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4aaff-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4aaff-126">接受</span><span class="sxs-lookup"><span data-stu-id="4aaff-126">Accept</span></span>|<span data-ttu-id="4aaff-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4aaff-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4aaff-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aaff-128">Request body</span></span>
<span data-ttu-id="4aaff-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4aaff-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aaff-130">响应</span><span class="sxs-lookup"><span data-stu-id="4aaff-130">Response</span></span>
<span data-ttu-id="4aaff-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4aaff-131">If successful, this method returns a `200 OK` response code and [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aaff-132">示例</span><span class="sxs-lookup"><span data-stu-id="4aaff-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="4aaff-133">请求</span><span class="sxs-lookup"><span data-stu-id="4aaff-133">Request</span></span>
<span data-ttu-id="4aaff-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4aaff-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="4aaff-135">响应</span><span class="sxs-lookup"><span data-stu-id="4aaff-135">Response</span></span>
<span data-ttu-id="4aaff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4aaff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": {
    "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
    "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
    "content": "Y29udGVudA==",
    "status": "provisioned",
    "password": "Password value",
    "subjectName": "Subject Name value",
    "subject": "Subject value",
    "issuerName": "Issuer Name value",
    "issuer": "Issuer value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
  }
}
```





