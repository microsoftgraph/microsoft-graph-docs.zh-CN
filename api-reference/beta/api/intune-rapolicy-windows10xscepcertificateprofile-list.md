---
title: 列出 windows10XSCEPCertificateProfiles
description: 列出 windows10XSCEPCertificateProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92cf38cb3557eea1fc7742a6a0726171884dbd61
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241557"
---
# <a name="list-windows10xscepcertificateprofiles"></a><span data-ttu-id="9c0c9-103">列出 windows10XSCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="9c0c9-103">List windows10XSCEPCertificateProfiles</span></span>

<span data-ttu-id="9c0c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c0c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c0c9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c0c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c0c9-107">列出 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-107">List properties and relationships of the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c0c9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9c0c9-108">Prerequisites</span></span>
<span data-ttu-id="9c0c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c0c9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9c0c9-111">Permission type</span></span>|<span data-ttu-id="9c0c9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9c0c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c0c9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9c0c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9c0c9-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c0c9-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9c0c9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9c0c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c0c9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-116">Not supported.</span></span>|
|<span data-ttu-id="9c0c9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9c0c9-117">Application</span></span>|<span data-ttu-id="9c0c9-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c0c9-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c0c9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9c0c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9c0c9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9c0c9-120">Request headers</span></span>
|<span data-ttu-id="9c0c9-121">标头</span><span class="sxs-lookup"><span data-stu-id="9c0c9-121">Header</span></span>|<span data-ttu-id="9c0c9-122">值</span><span class="sxs-lookup"><span data-stu-id="9c0c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c0c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c0c9-123">Authorization</span></span>|<span data-ttu-id="9c0c9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c0c9-125">接受</span><span class="sxs-lookup"><span data-stu-id="9c0c9-125">Accept</span></span>|<span data-ttu-id="9c0c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9c0c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c0c9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9c0c9-127">Request body</span></span>
<span data-ttu-id="9c0c9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c0c9-129">响应</span><span class="sxs-lookup"><span data-stu-id="9c0c9-129">Response</span></span>
<span data-ttu-id="9c0c9-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c0c9-131">示例</span><span class="sxs-lookup"><span data-stu-id="9c0c9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c0c9-132">请求</span><span class="sxs-lookup"><span data-stu-id="9c0c9-132">Request</span></span>
<span data-ttu-id="9c0c9-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="9c0c9-134">响应</span><span class="sxs-lookup"><span data-stu-id="9c0c9-134">Response</span></span>
<span data-ttu-id="9c0c9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9c0c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
      "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "certificateStore": "machine",
      "certificateValidityPeriodScale": "months",
      "certificateValidityPeriodValue": 14,
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "hashAlgorithm": [
        "sha2"
      ],
      "keySize": "size2048",
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "keyUsage": "digitalSignature",
      "renewalThresholdPercentage": 10,
      "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectAlternativeNameFormats": [
        {
          "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ],
      "subjectNameFormatString": "Subject Name Format String value"
    }
  ]
}
```




