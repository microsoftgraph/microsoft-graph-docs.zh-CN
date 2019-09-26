---
title: getEncryptionPublicKey 函数
description: 获取用于加密 Apple 设备注册计划令牌的公钥
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 78bf70af97c5964f55d24bed1f4d83e9a1ad2c56
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185327"
---
# <a name="getencryptionpublickey-function"></a><span data-ttu-id="c018e-103">getEncryptionPublicKey 函数</span><span class="sxs-lookup"><span data-stu-id="c018e-103">getEncryptionPublicKey function</span></span>

> <span data-ttu-id="c018e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c018e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c018e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c018e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c018e-106">获取用于加密 Apple 设备注册计划令牌的公钥</span><span class="sxs-lookup"><span data-stu-id="c018e-106">Get a public key to use to encrypt the Apple device enrollment program token</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c018e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c018e-107">Prerequisites</span></span>
<span data-ttu-id="c018e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c018e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c018e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c018e-110">Permission type</span></span>|<span data-ttu-id="c018e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c018e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c018e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c018e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c018e-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c018e-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c018e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c018e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c018e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c018e-115">Not supported.</span></span>|
|<span data-ttu-id="c018e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c018e-116">Application</span></span>|<span data-ttu-id="c018e-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c018e-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c018e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c018e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

## <a name="request-headers"></a><span data-ttu-id="c018e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c018e-119">Request headers</span></span>
|<span data-ttu-id="c018e-120">标头</span><span class="sxs-lookup"><span data-stu-id="c018e-120">Header</span></span>|<span data-ttu-id="c018e-121">值</span><span class="sxs-lookup"><span data-stu-id="c018e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c018e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c018e-122">Authorization</span></span>|<span data-ttu-id="c018e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c018e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c018e-124">接受</span><span class="sxs-lookup"><span data-stu-id="c018e-124">Accept</span></span>|<span data-ttu-id="c018e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c018e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c018e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c018e-126">Request body</span></span>
<span data-ttu-id="c018e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c018e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c018e-128">响应</span><span class="sxs-lookup"><span data-stu-id="c018e-128">Response</span></span>
<span data-ttu-id="c018e-129">如果成功，此函数会在`200 OK`响应正文中返回响应代码和字符串。</span><span class="sxs-lookup"><span data-stu-id="c018e-129">If successful, this function returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c018e-130">示例</span><span class="sxs-lookup"><span data-stu-id="c018e-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="c018e-131">请求</span><span class="sxs-lookup"><span data-stu-id="c018e-131">Request</span></span>
<span data-ttu-id="c018e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c018e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/getEncryptionPublicKey
```

### <a name="response"></a><span data-ttu-id="c018e-133">响应</span><span class="sxs-lookup"><span data-stu-id="c018e-133">Response</span></span>
<span data-ttu-id="c018e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c018e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 50

{
  "value": "Get Encryption Public Key value"
}
```




