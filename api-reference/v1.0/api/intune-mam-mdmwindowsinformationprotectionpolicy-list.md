---
title: 列出 mdmWindowsInformationProtectionPolicies
description: 列出 mdmWindowsInformationProtectionPolicy 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f35ee9d7663fc6cfcec92aafe33ce376952f0de
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981684"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="3d99d-103">列出 mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="3d99d-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="3d99d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3d99d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d99d-105">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d99d-105">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d99d-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d99d-106">Prerequisites</span></span>
<span data-ttu-id="3d99d-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="3d99d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d99d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d99d-109">Permission type</span></span>|<span data-ttu-id="3d99d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d99d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d99d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d99d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d99d-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d99d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3d99d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d99d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d99d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d99d-114">Not supported.</span></span>|
|<span data-ttu-id="3d99d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d99d-115">Application</span></span>|<span data-ttu-id="3d99d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d99d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d99d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d99d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3d99d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d99d-118">Request headers</span></span>
|<span data-ttu-id="3d99d-119">标头</span><span class="sxs-lookup"><span data-stu-id="3d99d-119">Header</span></span>|<span data-ttu-id="3d99d-120">值</span><span class="sxs-lookup"><span data-stu-id="3d99d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d99d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d99d-121">Authorization</span></span>|<span data-ttu-id="3d99d-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d99d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d99d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3d99d-123">Accept</span></span>|<span data-ttu-id="3d99d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d99d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d99d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d99d-125">Request body</span></span>
<span data-ttu-id="3d99d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d99d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d99d-127">响应</span><span class="sxs-lookup"><span data-stu-id="3d99d-127">Response</span></span>
<span data-ttu-id="3d99d-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3d99d-128">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d99d-129">示例</span><span class="sxs-lookup"><span data-stu-id="3d99d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d99d-130">请求</span><span class="sxs-lookup"><span data-stu-id="3d99d-130">Request</span></span>
<span data-ttu-id="3d99d-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d99d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="3d99d-132">响应</span><span class="sxs-lookup"><span data-stu-id="3d99d-132">Response</span></span>
<span data-ttu-id="3d99d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d99d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



