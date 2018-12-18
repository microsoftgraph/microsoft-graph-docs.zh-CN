---
title: 列表 windowsCertificateProfileBases
description: 列出属性和 windowsCertificateProfileBase 对象之间的关系。
author: tfitzmac
ms.openlocfilehash: 9fc17abe0b874cd360e94d1a28115823724c6f2d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344875"
---
# <a name="list-windowscertificateprofilebases"></a><span data-ttu-id="41495-103">列表 windowsCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="41495-103">List windowsCertificateProfileBases</span></span>

> <span data-ttu-id="41495-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="41495-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41495-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="41495-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41495-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41495-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41495-107">列出属性和[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="41495-107">List properties and relationships of the [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41495-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="41495-108">Prerequisites</span></span>
<span data-ttu-id="41495-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="41495-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41495-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="41495-111">Permission type</span></span>|<span data-ttu-id="41495-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41495-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41495-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41495-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41495-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="41495-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="41495-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41495-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41495-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="41495-116">Not supported.</span></span>|
|<span data-ttu-id="41495-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="41495-117">Application</span></span>|<span data-ttu-id="41495-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="41495-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41495-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41495-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41495-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="41495-120">Request headers</span></span>
|<span data-ttu-id="41495-121">标头</span><span class="sxs-lookup"><span data-stu-id="41495-121">Header</span></span>|<span data-ttu-id="41495-122">值</span><span class="sxs-lookup"><span data-stu-id="41495-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41495-123">授权</span><span class="sxs-lookup"><span data-stu-id="41495-123">Authorization</span></span>|<span data-ttu-id="41495-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41495-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41495-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41495-125">Accept</span></span>|<span data-ttu-id="41495-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41495-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41495-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41495-127">Request body</span></span>
<span data-ttu-id="41495-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41495-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41495-129">响应</span><span class="sxs-lookup"><span data-stu-id="41495-129">Response</span></span>
<span data-ttu-id="41495-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="41495-130">If successful, this method returns a `200 OK` response code and a collection of [windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41495-131">示例</span><span class="sxs-lookup"><span data-stu-id="41495-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="41495-132">请求</span><span class="sxs-lookup"><span data-stu-id="41495-132">Request</span></span>
<span data-ttu-id="41495-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41495-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="41495-134">响应</span><span class="sxs-lookup"><span data-stu-id="41495-134">Response</span></span>
<span data-ttu-id="41495-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41495-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsCertificateProfileBase",
      "id": "c0979ce1-9ce1-c097-e19c-97c0e19c97c0",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months"
    }
  ]
}
```





