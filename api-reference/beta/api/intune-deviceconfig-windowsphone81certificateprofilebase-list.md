---
title: 列出 windowsPhone81CertificateProfileBases
description: 列出 windowsPhone81CertificateProfileBase 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 33c17c0c6017d9a2eaf0e573e9ae3c880a60d40c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30982537"
---
# <a name="list-windowsphone81certificateprofilebases"></a><span data-ttu-id="02f00-103">列出 windowsPhone81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="02f00-103">List windowsPhone81CertificateProfileBases</span></span>

> <span data-ttu-id="02f00-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02f00-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02f00-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02f00-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02f00-106">列出[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="02f00-106">List properties and relationships of the [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02f00-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="02f00-107">Prerequisites</span></span>
<span data-ttu-id="02f00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02f00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f00-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="02f00-110">Permission type</span></span>|<span data-ttu-id="02f00-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02f00-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02f00-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02f00-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02f00-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02f00-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="02f00-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02f00-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02f00-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="02f00-115">Not supported.</span></span>|
|<span data-ttu-id="02f00-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="02f00-116">Application</span></span>|<span data-ttu-id="02f00-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="02f00-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02f00-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02f00-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="02f00-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="02f00-119">Request headers</span></span>
|<span data-ttu-id="02f00-120">标头</span><span class="sxs-lookup"><span data-stu-id="02f00-120">Header</span></span>|<span data-ttu-id="02f00-121">值</span><span class="sxs-lookup"><span data-stu-id="02f00-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02f00-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f00-122">Authorization</span></span>|<span data-ttu-id="02f00-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02f00-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02f00-124">接受</span><span class="sxs-lookup"><span data-stu-id="02f00-124">Accept</span></span>|<span data-ttu-id="02f00-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02f00-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02f00-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="02f00-126">Request body</span></span>
<span data-ttu-id="02f00-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="02f00-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02f00-128">响应</span><span class="sxs-lookup"><span data-stu-id="02f00-128">Response</span></span>
<span data-ttu-id="02f00-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="02f00-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02f00-130">示例</span><span class="sxs-lookup"><span data-stu-id="02f00-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02f00-131">请求</span><span class="sxs-lookup"><span data-stu-id="02f00-131">Request</span></span>
<span data-ttu-id="02f00-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02f00-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="02f00-133">响应</span><span class="sxs-lookup"><span data-stu-id="02f00-133">Response</span></span>
<span data-ttu-id="02f00-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02f00-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1030

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CertificateProfileBase",
      "id": "336e97ac-97ac-336e-ac97-6e33ac976e33",
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
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ]
    }
  ]
}
```




