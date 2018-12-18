---
title: 删除 windowsPhone81TrustedRootCertificate
description: 删除 windowsPhone81TrustedRootCertificate。
author: tfitzmac
ms.openlocfilehash: 5a290ccc5f8597c461d63f48ded49ef20fdcb082
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302420"
---
# <a name="delete-windowsphone81trustedrootcertificate"></a><span data-ttu-id="bef20-103">删除 windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="bef20-103">Delete windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="bef20-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bef20-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bef20-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bef20-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bef20-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bef20-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bef20-107">删除[windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="bef20-107">Deletes a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bef20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bef20-108">Prerequisites</span></span>
<span data-ttu-id="bef20-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="bef20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bef20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bef20-111">Permission type</span></span>|<span data-ttu-id="bef20-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bef20-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bef20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bef20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bef20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bef20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bef20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bef20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bef20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bef20-116">Not supported.</span></span>|
|<span data-ttu-id="bef20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bef20-117">Application</span></span>|<span data-ttu-id="bef20-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bef20-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bef20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bef20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="bef20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bef20-120">Request headers</span></span>
|<span data-ttu-id="bef20-121">标头</span><span class="sxs-lookup"><span data-stu-id="bef20-121">Header</span></span>|<span data-ttu-id="bef20-122">值</span><span class="sxs-lookup"><span data-stu-id="bef20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bef20-123">授权</span><span class="sxs-lookup"><span data-stu-id="bef20-123">Authorization</span></span>|<span data-ttu-id="bef20-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bef20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bef20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bef20-125">Accept</span></span>|<span data-ttu-id="bef20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bef20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bef20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bef20-127">Request body</span></span>
<span data-ttu-id="bef20-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bef20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bef20-129">响应</span><span class="sxs-lookup"><span data-stu-id="bef20-129">Response</span></span>
<span data-ttu-id="bef20-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bef20-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bef20-131">示例</span><span class="sxs-lookup"><span data-stu-id="bef20-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bef20-132">请求</span><span class="sxs-lookup"><span data-stu-id="bef20-132">Request</span></span>
<span data-ttu-id="bef20-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bef20-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="bef20-134">响应</span><span class="sxs-lookup"><span data-stu-id="bef20-134">Response</span></span>
<span data-ttu-id="bef20-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bef20-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





