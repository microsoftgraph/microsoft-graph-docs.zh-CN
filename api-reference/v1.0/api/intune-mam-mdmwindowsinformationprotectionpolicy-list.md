---
title: 列出 mdmWindowsInformationProtectionPolicies
description: 列出 mdmWindowsInformationProtectionPolicy 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 41b25c7bd955026455337073a0d1c8eb8e010921
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257762"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="90dac-103">列出 mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="90dac-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="90dac-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90dac-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90dac-105">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="90dac-105">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90dac-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="90dac-106">Prerequisites</span></span>
<span data-ttu-id="90dac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="90dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="90dac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="90dac-109">Permission type</span></span>|<span data-ttu-id="90dac-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="90dac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90dac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90dac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90dac-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="90dac-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="90dac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90dac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90dac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="90dac-114">Not supported.</span></span>|
|<span data-ttu-id="90dac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="90dac-115">Application</span></span>|<span data-ttu-id="90dac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90dac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90dac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90dac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="90dac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="90dac-118">Request headers</span></span>
|<span data-ttu-id="90dac-119">标头</span><span class="sxs-lookup"><span data-stu-id="90dac-119">Header</span></span>|<span data-ttu-id="90dac-120">值</span><span class="sxs-lookup"><span data-stu-id="90dac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90dac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90dac-121">Authorization</span></span>|<span data-ttu-id="90dac-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="90dac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90dac-123">Accept</span><span class="sxs-lookup"><span data-stu-id="90dac-123">Accept</span></span>|<span data-ttu-id="90dac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90dac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90dac-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="90dac-125">Request body</span></span>
<span data-ttu-id="90dac-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90dac-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90dac-127">响应</span><span class="sxs-lookup"><span data-stu-id="90dac-127">Response</span></span>
<span data-ttu-id="90dac-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90dac-128">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90dac-129">示例</span><span class="sxs-lookup"><span data-stu-id="90dac-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="90dac-130">请求</span><span class="sxs-lookup"><span data-stu-id="90dac-130">Request</span></span>
<span data-ttu-id="90dac-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="90dac-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="90dac-132">响应</span><span class="sxs-lookup"><span data-stu-id="90dac-132">Response</span></span>
<span data-ttu-id="90dac-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="90dac-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4610

{
  "value": [
    {
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
  ]
}
```



