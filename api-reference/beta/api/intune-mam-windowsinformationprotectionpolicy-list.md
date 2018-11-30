---
title: 列出 windowsInformationProtectionPolicies
description: 列出 windowsInformationProtectionPolicy 对象的属性和关系。
ms.openlocfilehash: 98d6817bd53a695bdac1cf1902063e4c3c1252d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049453"
---
# <a name="list-windowsinformationprotectionpolicies"></a><span data-ttu-id="21f4b-103">列出 windowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="21f4b-103">List windowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="21f4b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="21f4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21f4b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21f4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21f4b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="21f4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21f4b-107">列出 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="21f4b-107">List properties and relationships of the [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="21f4b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="21f4b-108">Prerequisites</span></span>
<span data-ttu-id="21f4b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="21f4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21f4b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="21f4b-111">Permission type</span></span>|<span data-ttu-id="21f4b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="21f4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21f4b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21f4b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21f4b-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="21f4b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="21f4b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21f4b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21f4b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21f4b-116">Not supported.</span></span>|
|<span data-ttu-id="21f4b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="21f4b-117">Application</span></span>|<span data-ttu-id="21f4b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="21f4b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21f4b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21f4b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="21f4b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="21f4b-120">Request headers</span></span>
|<span data-ttu-id="21f4b-121">标头</span><span class="sxs-lookup"><span data-stu-id="21f4b-121">Header</span></span>|<span data-ttu-id="21f4b-122">值</span><span class="sxs-lookup"><span data-stu-id="21f4b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21f4b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21f4b-123">Authorization</span></span>|<span data-ttu-id="21f4b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="21f4b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21f4b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="21f4b-125">Accept</span></span>|<span data-ttu-id="21f4b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21f4b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21f4b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="21f4b-127">Request body</span></span>
<span data-ttu-id="21f4b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21f4b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21f4b-129">响应</span><span class="sxs-lookup"><span data-stu-id="21f4b-129">Response</span></span>
<span data-ttu-id="21f4b-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="21f4b-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21f4b-131">示例</span><span class="sxs-lookup"><span data-stu-id="21f4b-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="21f4b-132">请求</span><span class="sxs-lookup"><span data-stu-id="21f4b-132">Request</span></span>
<span data-ttu-id="21f4b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="21f4b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="21f4b-134">响应</span><span class="sxs-lookup"><span data-stu-id="21f4b-134">Response</span></span>
<span data-ttu-id="21f4b-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="21f4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5158

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





