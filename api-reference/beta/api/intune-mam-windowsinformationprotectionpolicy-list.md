---
title: 列出 windowsInformationProtectionPolicies
description: 列出 windowsInformationProtectionPolicy 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a7ca65e4d95b02ae71476e47a3186086fc007f3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145729"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="a67fa-103">列出 windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="a67fa-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="a67fa-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a67fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a67fa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a67fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a67fa-106">列出 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a67fa-106">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a67fa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a67fa-107">Prerequisites</span></span>
<span data-ttu-id="a67fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a67fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a67fa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a67fa-110">Permission type</span></span>|<span data-ttu-id="a67fa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a67fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a67fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a67fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a67fa-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a67fa-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a67fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a67fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a67fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a67fa-115">Not supported.</span></span>|
|<span data-ttu-id="a67fa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a67fa-116">Application</span></span>|<span data-ttu-id="a67fa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a67fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a67fa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a67fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a67fa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a67fa-119">Request headers</span></span>
|<span data-ttu-id="a67fa-120">标头</span><span class="sxs-lookup"><span data-stu-id="a67fa-120">Header</span></span>|<span data-ttu-id="a67fa-121">值</span><span class="sxs-lookup"><span data-stu-id="a67fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a67fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a67fa-122">Authorization</span></span>|<span data-ttu-id="a67fa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a67fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a67fa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a67fa-124">Accept</span></span>|<span data-ttu-id="a67fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a67fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a67fa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a67fa-126">Request body</span></span>
<span data-ttu-id="a67fa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a67fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a67fa-128">响应</span><span class="sxs-lookup"><span data-stu-id="a67fa-128">Response</span></span>
<span data-ttu-id="a67fa-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a67fa-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a67fa-130">示例</span><span class="sxs-lookup"><span data-stu-id="a67fa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a67fa-131">请求</span><span class="sxs-lookup"><span data-stu-id="a67fa-131">Request</span></span>
<span data-ttu-id="a67fa-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a67fa-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="a67fa-133">响应</span><span class="sxs-lookup"><span data-stu-id="a67fa-133">Response</span></span>
<span data-ttu-id="a67fa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a67fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5232

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "6397be61-be61-6397-61be-976361be9763",
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
      "isAssigned": true,
      "revokeOnMdmHandoffDisabled": true,
      "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
      "windowsHelloForBusinessBlocked": true,
      "pinMinimumLength": 0,
      "pinUppercaseLetters": "requireAtLeastOne",
      "pinLowercaseLetters": "requireAtLeastOne",
      "pinSpecialCharacters": "requireAtLeastOne",
      "pinExpirationDays": 1,
      "numberOfPastPinsRemembered": 10,
      "passwordMaximumAttemptCount": 11,
      "minutesOfInactivityBeforeDeviceLock": 3,
      "daysWithoutContactBeforeUnenroll": 0
    }
  ]
}
```




