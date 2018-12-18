---
title: 删除 iosTrustedRootCertificate
description: 删除 iosTrustedRootCertificate。
author: tfitzmac
ms.openlocfilehash: f83669c4eb196ecd9de64c3be365301c388bdf5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362592"
---
# <a name="delete-iostrustedrootcertificate"></a><span data-ttu-id="0e619-103">删除 iosTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="0e619-103">Delete iosTrustedRootCertificate</span></span>

> <span data-ttu-id="0e619-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e619-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e619-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e619-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e619-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e619-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e619-107">删除[iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="0e619-107">Deletes a [iosTrustedRootCertificate](../resources/intune-deviceconfig-iostrustedrootcertificate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e619-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e619-108">Prerequisites</span></span>
<span data-ttu-id="0e619-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0e619-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e619-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e619-111">Permission type</span></span>|<span data-ttu-id="0e619-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e619-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e619-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e619-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e619-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e619-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e619-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e619-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e619-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e619-116">Not supported.</span></span>|
|<span data-ttu-id="0e619-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e619-117">Application</span></span>|<span data-ttu-id="0e619-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e619-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e619-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e619-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosEnterpriseWiFiConfiguration/rootCertificatesForServerValidation/{iosTrustedRootCertificateId}
```

## <a name="request-headers"></a><span data-ttu-id="0e619-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e619-120">Request headers</span></span>
|<span data-ttu-id="0e619-121">标头</span><span class="sxs-lookup"><span data-stu-id="0e619-121">Header</span></span>|<span data-ttu-id="0e619-122">值</span><span class="sxs-lookup"><span data-stu-id="0e619-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e619-123">授权</span><span class="sxs-lookup"><span data-stu-id="0e619-123">Authorization</span></span>|<span data-ttu-id="0e619-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e619-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e619-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e619-125">Accept</span></span>|<span data-ttu-id="0e619-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e619-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e619-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e619-127">Request body</span></span>
<span data-ttu-id="0e619-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0e619-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e619-129">响应</span><span class="sxs-lookup"><span data-stu-id="0e619-129">Response</span></span>
<span data-ttu-id="0e619-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0e619-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0e619-131">示例</span><span class="sxs-lookup"><span data-stu-id="0e619-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e619-132">请求</span><span class="sxs-lookup"><span data-stu-id="0e619-132">Request</span></span>
<span data-ttu-id="0e619-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e619-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="0e619-134">响应</span><span class="sxs-lookup"><span data-stu-id="0e619-134">Response</span></span>
<span data-ttu-id="0e619-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e619-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





