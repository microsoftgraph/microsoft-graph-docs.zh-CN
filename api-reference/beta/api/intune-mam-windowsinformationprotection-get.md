---
title: 获取 windowsInformationProtection
description: 读取 windowsInformationProtection 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c319b699ac70db6d26d2d4030c3b427f6540343
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148895"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="292d3-103">获取 windowsInformationProtection</span><span class="sxs-lookup"><span data-stu-id="292d3-103">Get windowsInformationProtection</span></span>

<span data-ttu-id="292d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="292d3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="292d3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="292d3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="292d3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="292d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="292d3-107">读取 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="292d3-107">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="292d3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="292d3-108">Prerequisites</span></span>
<span data-ttu-id="292d3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="292d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="292d3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="292d3-111">Permission type</span></span>|<span data-ttu-id="292d3-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="292d3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="292d3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="292d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="292d3-114">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292d3-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="292d3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="292d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="292d3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="292d3-116">Not supported.</span></span>|
|<span data-ttu-id="292d3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="292d3-117">Application</span></span>|<span data-ttu-id="292d3-118">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="292d3-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="292d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="292d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="292d3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="292d3-120">Optional query parameters</span></span>
<span data-ttu-id="292d3-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="292d3-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="292d3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="292d3-122">Request headers</span></span>
|<span data-ttu-id="292d3-123">标头</span><span class="sxs-lookup"><span data-stu-id="292d3-123">Header</span></span>|<span data-ttu-id="292d3-124">值</span><span class="sxs-lookup"><span data-stu-id="292d3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="292d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="292d3-125">Authorization</span></span>|<span data-ttu-id="292d3-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="292d3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="292d3-127">接受</span><span class="sxs-lookup"><span data-stu-id="292d3-127">Accept</span></span>|<span data-ttu-id="292d3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="292d3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="292d3-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="292d3-129">Request body</span></span>
<span data-ttu-id="292d3-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="292d3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="292d3-131">响应</span><span class="sxs-lookup"><span data-stu-id="292d3-131">Response</span></span>
<span data-ttu-id="292d3-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="292d3-132">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="292d3-133">示例</span><span class="sxs-lookup"><span data-stu-id="292d3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="292d3-134">请求</span><span class="sxs-lookup"><span data-stu-id="292d3-134">Request</span></span>
<span data-ttu-id="292d3-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="292d3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="292d3-136">响应</span><span class="sxs-lookup"><span data-stu-id="292d3-136">Response</span></span>
<span data-ttu-id="292d3-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="292d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4299

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "ca339419-9419-ca33-1994-33ca199433ca",
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
            "@odata.type": "microsoft.graph.ipRange"
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




