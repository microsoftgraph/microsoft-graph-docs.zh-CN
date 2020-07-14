---
title: 获取 managedAllDeviceCertificateState
description: 读取 managedAllDeviceCertificateState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2a6d362e06a81014fcc5d20b24ad4779544b5410
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45122978"
---
# <a name="get-managedalldevicecertificatestate"></a><span data-ttu-id="943bc-103">获取 managedAllDeviceCertificateState</span><span class="sxs-lookup"><span data-stu-id="943bc-103">Get managedAllDeviceCertificateState</span></span>

<span data-ttu-id="943bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="943bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="943bc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="943bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="943bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="943bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="943bc-107">读取[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="943bc-107">Read properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="943bc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="943bc-108">Prerequisites</span></span>
<span data-ttu-id="943bc-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="943bc-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="943bc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="943bc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="943bc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="943bc-111">Permission type</span></span>|<span data-ttu-id="943bc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="943bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="943bc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="943bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="943bc-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="943bc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="943bc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="943bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="943bc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="943bc-116">Not supported.</span></span>|
|<span data-ttu-id="943bc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="943bc-117">Application</span></span>|<span data-ttu-id="943bc-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="943bc-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="943bc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="943bc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="943bc-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="943bc-120">Optional query parameters</span></span>
<span data-ttu-id="943bc-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="943bc-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="943bc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="943bc-122">Request headers</span></span>
|<span data-ttu-id="943bc-123">标头</span><span class="sxs-lookup"><span data-stu-id="943bc-123">Header</span></span>|<span data-ttu-id="943bc-124">值</span><span class="sxs-lookup"><span data-stu-id="943bc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="943bc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="943bc-125">Authorization</span></span>|<span data-ttu-id="943bc-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="943bc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="943bc-127">接受</span><span class="sxs-lookup"><span data-stu-id="943bc-127">Accept</span></span>|<span data-ttu-id="943bc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="943bc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="943bc-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="943bc-129">Request body</span></span>
<span data-ttu-id="943bc-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="943bc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="943bc-131">响应</span><span class="sxs-lookup"><span data-stu-id="943bc-131">Response</span></span>
<span data-ttu-id="943bc-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="943bc-132">If successful, this method returns a `200 OK` response code and [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="943bc-133">示例</span><span class="sxs-lookup"><span data-stu-id="943bc-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="943bc-134">请求</span><span class="sxs-lookup"><span data-stu-id="943bc-134">Request</span></span>
<span data-ttu-id="943bc-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="943bc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates/{managedAllDeviceCertificateStateId}
```

### <a name="response"></a><span data-ttu-id="943bc-136">响应</span><span class="sxs-lookup"><span data-stu-id="943bc-136">Response</span></span>
<span data-ttu-id="943bc-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="943bc-137">Here is an example of the response.</span></span> <span data-ttu-id="943bc-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="943bc-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="943bc-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="943bc-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 916

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
    "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
    "certificateRevokeStatus": "pending",
    "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:34.9547208-08:00",
    "managedDeviceDisplayName": "Managed Device Display Name value",
    "userPrincipalName": "User Principal Name value",
    "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
    "certificateIssuerName": "Certificate Issuer Name value",
    "certificateThumbprint": "Certificate Thumbprint value",
    "certificateSerialNumber": "Certificate Serial Number value",
    "certificateSubjectName": "Certificate Subject Name value",
    "certificateKeyUsages": 4,
    "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
    "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00"
  }
}
```



