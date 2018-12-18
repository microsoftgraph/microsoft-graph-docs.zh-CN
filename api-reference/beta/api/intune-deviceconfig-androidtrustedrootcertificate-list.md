---
title: 列表 androidTrustedRootCertificates
description: 列出属性和 androidTrustedRootCertificate 对象之间的关系。
author: tfitzmac
ms.openlocfilehash: e03e46c8029014e83aed06c5c9b9327fec37121a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347773"
---
# <a name="list-androidtrustedrootcertificates"></a><span data-ttu-id="1038d-103">列表 androidTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="1038d-103">List androidTrustedRootCertificates</span></span>

> <span data-ttu-id="1038d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1038d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1038d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1038d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1038d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1038d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1038d-107">列出属性和[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="1038d-107">List properties and relationships of the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1038d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1038d-108">Prerequisites</span></span>
<span data-ttu-id="1038d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1038d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1038d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1038d-111">Permission type</span></span>|<span data-ttu-id="1038d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1038d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1038d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1038d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1038d-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1038d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1038d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1038d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1038d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1038d-116">Not supported.</span></span>|
|<span data-ttu-id="1038d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1038d-117">Application</span></span>|<span data-ttu-id="1038d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1038d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1038d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1038d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1038d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1038d-120">Request headers</span></span>
|<span data-ttu-id="1038d-121">标头</span><span class="sxs-lookup"><span data-stu-id="1038d-121">Header</span></span>|<span data-ttu-id="1038d-122">值</span><span class="sxs-lookup"><span data-stu-id="1038d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1038d-123">授权</span><span class="sxs-lookup"><span data-stu-id="1038d-123">Authorization</span></span>|<span data-ttu-id="1038d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1038d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1038d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1038d-125">Accept</span></span>|<span data-ttu-id="1038d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1038d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1038d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1038d-127">Request body</span></span>
<span data-ttu-id="1038d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1038d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1038d-129">响应</span><span class="sxs-lookup"><span data-stu-id="1038d-129">Response</span></span>
<span data-ttu-id="1038d-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1038d-130">If successful, this method returns a `200 OK` response code and a collection of [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1038d-131">示例</span><span class="sxs-lookup"><span data-stu-id="1038d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1038d-132">请求</span><span class="sxs-lookup"><span data-stu-id="1038d-132">Request</span></span>
<span data-ttu-id="1038d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1038d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1038d-134">响应</span><span class="sxs-lookup"><span data-stu-id="1038d-134">Response</span></span>
<span data-ttu-id="1038d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1038d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
      "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
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
      "certFileName": "Cert File Name value"
    }
  ]
}
```





