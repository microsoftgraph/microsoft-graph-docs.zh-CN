---
title: 列出 managedAllDeviceCertificateStates
description: 列出 managedAllDeviceCertificateState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9287bede55dcae67787e86758146dc9433f89d8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792721"
---
# <a name="list-managedalldevicecertificatestates"></a><span data-ttu-id="fbd64-103">列出 managedAllDeviceCertificateStates</span><span class="sxs-lookup"><span data-stu-id="fbd64-103">List managedAllDeviceCertificateStates</span></span>

<span data-ttu-id="fbd64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbd64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbd64-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fbd64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbd64-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fbd64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbd64-107">列出[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fbd64-107">List properties and relationships of the [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbd64-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fbd64-108">Prerequisites</span></span>
<span data-ttu-id="fbd64-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="fbd64-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="fbd64-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbd64-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbd64-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbd64-111">Permission type</span></span>|<span data-ttu-id="fbd64-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fbd64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbd64-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbd64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbd64-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbd64-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fbd64-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbd64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbd64-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbd64-116">Not supported.</span></span>|
|<span data-ttu-id="fbd64-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbd64-117">Application</span></span>|<span data-ttu-id="fbd64-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbd64-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbd64-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbd64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="fbd64-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fbd64-120">Request headers</span></span>
|<span data-ttu-id="fbd64-121">标头</span><span class="sxs-lookup"><span data-stu-id="fbd64-121">Header</span></span>|<span data-ttu-id="fbd64-122">值</span><span class="sxs-lookup"><span data-stu-id="fbd64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbd64-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbd64-123">Authorization</span></span>|<span data-ttu-id="fbd64-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fbd64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbd64-125">接受</span><span class="sxs-lookup"><span data-stu-id="fbd64-125">Accept</span></span>|<span data-ttu-id="fbd64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbd64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbd64-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbd64-127">Request body</span></span>
<span data-ttu-id="fbd64-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbd64-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbd64-129">响应</span><span class="sxs-lookup"><span data-stu-id="fbd64-129">Response</span></span>
<span data-ttu-id="fbd64-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="fbd64-130">If successful, this method returns a `200 OK` response code and a collection of [managedAllDeviceCertificateState](../resources/intune-deviceconfig-managedalldevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbd64-131">示例</span><span class="sxs-lookup"><span data-stu-id="fbd64-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbd64-132">请求</span><span class="sxs-lookup"><span data-stu-id="fbd64-132">Request</span></span>
<span data-ttu-id="fbd64-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbd64-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationsAllManagedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="fbd64-134">响应</span><span class="sxs-lookup"><span data-stu-id="fbd64-134">Response</span></span>
<span data-ttu-id="fbd64-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="fbd64-135">Here is an example of the response.</span></span> <span data-ttu-id="fbd64-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="fbd64-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fbd64-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="fbd64-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 869

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAllDeviceCertificateState",
      "id": "987c6a17-6a17-987c-176a-7c98176a7c98",
      "certificateRevokeStatus": "pending",
      "managedDeviceDisplayName": "Managed Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
      "certificateIssuerName": "Certificate Issuer Name value",
      "certificateThumbprint": "Certificate Thumbprint value",
      "certificateSerialNumber": "Certificate Serial Number value",
      "certificateSubjectName": "Certificate Subject Name value",
      "certificateKeyUsages": 4,
      "certificateExtendedKeyUsages": "Certificate Extended Key Usages value",
      "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
      "certificateRevokeStatusLastChangeDateTime": "2016-12-31T23:59:41.5044473-08:00"
    }
  ]
}
```



