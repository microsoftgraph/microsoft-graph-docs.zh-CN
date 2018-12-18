---
title: 删除 androidForWorkTrustedRootCertificate
description: 删除 androidForWorkTrustedRootCertificate。
author: tfitzmac
ms.openlocfilehash: 2571e3fd270ef56e8b93ea44efc826cf89a8613f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318031"
---
# <a name="delete-androidforworktrustedrootcertificate"></a><span data-ttu-id="a7ca6-103">删除 androidForWorkTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a7ca6-103">Delete androidForWorkTrustedRootCertificate</span></span>

> <span data-ttu-id="a7ca6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7ca6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7ca6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7ca6-107">删除[androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md)。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-107">Deletes a [androidForWorkTrustedRootCertificate](../resources/intune-deviceconfig-androidforworktrustedrootcertificate.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7ca6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a7ca6-108">Prerequisites</span></span>
<span data-ttu-id="a7ca6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a7ca6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7ca6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7ca6-111">Permission type</span></span>|<span data-ttu-id="a7ca6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a7ca6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7ca6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7ca6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7ca6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7ca6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7ca6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7ca6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7ca6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-116">Not supported.</span></span>|
|<span data-ttu-id="a7ca6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7ca6-117">Application</span></span>|<span data-ttu-id="a7ca6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7ca6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7ca6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="a7ca6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7ca6-120">Request headers</span></span>
|<span data-ttu-id="a7ca6-121">标头</span><span class="sxs-lookup"><span data-stu-id="a7ca6-121">Header</span></span>|<span data-ttu-id="a7ca6-122">值</span><span class="sxs-lookup"><span data-stu-id="a7ca6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7ca6-123">授权</span><span class="sxs-lookup"><span data-stu-id="a7ca6-123">Authorization</span></span>|<span data-ttu-id="a7ca6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7ca6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7ca6-125">Accept</span></span>|<span data-ttu-id="a7ca6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7ca6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7ca6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7ca6-127">Request body</span></span>
<span data-ttu-id="a7ca6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7ca6-129">响应</span><span class="sxs-lookup"><span data-stu-id="a7ca6-129">Response</span></span>
<span data-ttu-id="a7ca6-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a7ca6-131">示例</span><span class="sxs-lookup"><span data-stu-id="a7ca6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7ca6-132">请求</span><span class="sxs-lookup"><span data-stu-id="a7ca6-132">Request</span></span>
<span data-ttu-id="a7ca6-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate
```

### <a name="response"></a><span data-ttu-id="a7ca6-134">响应</span><span class="sxs-lookup"><span data-stu-id="a7ca6-134">Response</span></span>
<span data-ttu-id="a7ca6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7ca6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





