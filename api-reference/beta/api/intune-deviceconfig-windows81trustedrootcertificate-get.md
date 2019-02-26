---
title: 获取 windows81TrustedRootCertificate
description: 读取 windows81TrustedRootCertificate 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c61c108cb67f2a58535f0586b0dbe9de3eaae8f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163523"
---
# <a name="get-windows81trustedrootcertificate"></a><span data-ttu-id="ccc5e-103">获取 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ccc5e-103">Get windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="ccc5e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ccc5e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccc5e-106">读取[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-106">Read properties and relationships of the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ccc5e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ccc5e-107">Prerequisites</span></span>
<span data-ttu-id="ccc5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ccc5e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ccc5e-110">Permission type</span></span>|<span data-ttu-id="ccc5e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ccc5e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccc5e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc5e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ccc5e-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ccc5e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ccc5e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ccc5e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccc5e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-115">Not supported.</span></span>|
|<span data-ttu-id="ccc5e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ccc5e-116">Application</span></span>|<span data-ttu-id="ccc5e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccc5e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ccc5e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccc5e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ccc5e-119">Optional query parameters</span></span>
<span data-ttu-id="ccc5e-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccc5e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ccc5e-121">Request headers</span></span>
|<span data-ttu-id="ccc5e-122">标头</span><span class="sxs-lookup"><span data-stu-id="ccc5e-122">Header</span></span>|<span data-ttu-id="ccc5e-123">值</span><span class="sxs-lookup"><span data-stu-id="ccc5e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ccc5e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ccc5e-124">Authorization</span></span>|<span data-ttu-id="ccc5e-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ccc5e-126">Accept</span><span class="sxs-lookup"><span data-stu-id="ccc5e-126">Accept</span></span>|<span data-ttu-id="ccc5e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ccc5e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccc5e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ccc5e-128">Request body</span></span>
<span data-ttu-id="ccc5e-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccc5e-130">响应</span><span class="sxs-lookup"><span data-stu-id="ccc5e-130">Response</span></span>
<span data-ttu-id="ccc5e-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-131">If successful, this method returns a `200 OK` response code and [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ccc5e-132">示例</span><span class="sxs-lookup"><span data-stu-id="ccc5e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ccc5e-133">请求</span><span class="sxs-lookup"><span data-stu-id="ccc5e-133">Request</span></span>
<span data-ttu-id="ccc5e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
```

### <a name="response"></a><span data-ttu-id="ccc5e-135">响应</span><span class="sxs-lookup"><span data-stu-id="ccc5e-135">Response</span></span>
<span data-ttu-id="ccc5e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ccc5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
    "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
    "certFileName": "Cert File Name value",
    "destinationStore": "computerCertStoreIntermediate"
  }
}
```




