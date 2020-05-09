---
title: 删除 windows81TrustedRootCertificate
description: 删除 windows81TrustedRootCertificate。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4b7880ef06d54fe7010be0871619a2f07cb4118a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179016"
---
# <a name="delete-windows81trustedrootcertificate"></a><span data-ttu-id="8319b-103">删除 windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="8319b-103">Delete windows81TrustedRootCertificate</span></span>

<span data-ttu-id="8319b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8319b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8319b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8319b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8319b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8319b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8319b-107">删除[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="8319b-107">Deletes a [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8319b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="8319b-108">Prerequisites</span></span>
<span data-ttu-id="8319b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8319b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8319b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="8319b-111">Permission type</span></span>|<span data-ttu-id="8319b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8319b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8319b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8319b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8319b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8319b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8319b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8319b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8319b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8319b-116">Not supported.</span></span>|
|<span data-ttu-id="8319b-117">Application</span><span class="sxs-lookup"><span data-stu-id="8319b-117">Application</span></span>|<span data-ttu-id="8319b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8319b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8319b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8319b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="8319b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8319b-120">Request headers</span></span>
|<span data-ttu-id="8319b-121">标头</span><span class="sxs-lookup"><span data-stu-id="8319b-121">Header</span></span>|<span data-ttu-id="8319b-122">值</span><span class="sxs-lookup"><span data-stu-id="8319b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8319b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8319b-123">Authorization</span></span>|<span data-ttu-id="8319b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8319b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8319b-125">接受</span><span class="sxs-lookup"><span data-stu-id="8319b-125">Accept</span></span>|<span data-ttu-id="8319b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8319b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8319b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8319b-127">Request body</span></span>
<span data-ttu-id="8319b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8319b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8319b-129">响应</span><span class="sxs-lookup"><span data-stu-id="8319b-129">Response</span></span>
<span data-ttu-id="8319b-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="8319b-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8319b-131">示例</span><span class="sxs-lookup"><span data-stu-id="8319b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8319b-132">请求</span><span class="sxs-lookup"><span data-stu-id="8319b-132">Request</span></span>
<span data-ttu-id="8319b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8319b-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificateForClientValidation
```

### <a name="response"></a><span data-ttu-id="8319b-134">响应</span><span class="sxs-lookup"><span data-stu-id="8319b-134">Response</span></span>
<span data-ttu-id="8319b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8319b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



