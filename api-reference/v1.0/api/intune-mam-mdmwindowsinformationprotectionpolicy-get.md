---
title: 获取 mdmWindowsInformationProtectionPolicy
description: 读取 mdmWindowsInformationProtectionPolicy 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aef13a170092b0fa3902631e62d8f069f3e70b37
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756924"
---
# <a name="get-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="c6b82-103">获取 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="c6b82-103">Get mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="c6b82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6b82-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6b82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6b82-106">读取 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6b82-106">Read properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c6b82-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c6b82-107">Prerequisites</span></span>
<span data-ttu-id="c6b82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6b82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6b82-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6b82-110">Permission type</span></span>|<span data-ttu-id="c6b82-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6b82-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6b82-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6b82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c6b82-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b82-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c6b82-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6b82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6b82-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6b82-115">Not supported.</span></span>|
|<span data-ttu-id="c6b82-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6b82-116">Application</span></span>|<span data-ttu-id="c6b82-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6b82-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6b82-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6b82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c6b82-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c6b82-119">Optional query parameters</span></span>
<span data-ttu-id="c6b82-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c6b82-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c6b82-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6b82-121">Request headers</span></span>
|<span data-ttu-id="c6b82-122">标头</span><span class="sxs-lookup"><span data-stu-id="c6b82-122">Header</span></span>|<span data-ttu-id="c6b82-123">值</span><span class="sxs-lookup"><span data-stu-id="c6b82-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6b82-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6b82-124">Authorization</span></span>|<span data-ttu-id="c6b82-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c6b82-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6b82-126">接受</span><span class="sxs-lookup"><span data-stu-id="c6b82-126">Accept</span></span>|<span data-ttu-id="c6b82-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c6b82-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6b82-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6b82-128">Request body</span></span>
<span data-ttu-id="c6b82-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6b82-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6b82-130">响应</span><span class="sxs-lookup"><span data-stu-id="c6b82-130">Response</span></span>
<span data-ttu-id="c6b82-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6b82-131">If successful, this method returns a `200 OK` response code and [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6b82-132">示例</span><span class="sxs-lookup"><span data-stu-id="c6b82-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c6b82-133">请求</span><span class="sxs-lookup"><span data-stu-id="c6b82-133">Request</span></span>
<span data-ttu-id="c6b82-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6b82-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="c6b82-135">响应</span><span class="sxs-lookup"><span data-stu-id="c6b82-135">Response</span></span>
<span data-ttu-id="c6b82-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6b82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4346

{
  "value": {
    "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
    "version": "Version value",
    "enforcementLevel": "encryptAndAuditOnly",
    "enterpriseDomain": "Enterprise Domain value",
    "enterpriseProtectedDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "protectionUnderLockConfigRequired": true,
    "dataRecoveryCertificate": {
      "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
      "subjectName": "Subject Name value",
      "description": "Description value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "certificate": "Y2VydGlmaWNhdGU="
    },
    "revokeOnUnenrollDisabled": true,
    "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
    "azureRightsManagementServicesAllowed": true,
    "iconsVisible": true,
    "protectedApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "exemptApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "enterpriseNetworkDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxiedDomains": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
        "displayName": "Display Name value",
        "proxiedDomains": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ]
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
        "displayName": "Display Name value",
        "ranges": [
          {
            "@odata.type": "microsoft.graph.iPv6Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ]
      }
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseInternalProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "indexingEncryptedStoresOrItemsBlocked": true,
    "smbAutoEncryptedFileExtensions": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "isAssigned": true
  }
}
```




