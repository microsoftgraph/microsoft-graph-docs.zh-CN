---
title: 列出 mdmWindowsInformationProtectionPolicies
description: 列出 mdmWindowsInformationProtectionPolicy 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f74cc570cccaa3206d81f82f22e07dc253d68dfb
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863035"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="ec60d-103">列出 mdmWindowsInformationProtectionPolicies</span><span class="sxs-lookup"><span data-stu-id="ec60d-103">List mdmWindowsInformationProtectionPolicies</span></span>

<span data-ttu-id="ec60d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec60d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec60d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec60d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec60d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec60d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec60d-107">列出 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ec60d-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec60d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec60d-108">Prerequisites</span></span>
<span data-ttu-id="ec60d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec60d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec60d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec60d-111">Permission type</span></span>|<span data-ttu-id="ec60d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec60d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec60d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec60d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ec60d-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="ec60d-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ec60d-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec60d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="ec60d-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="ec60d-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ec60d-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec60d-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ec60d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec60d-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec60d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec60d-119">Not supported.</span></span>|
|<span data-ttu-id="ec60d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec60d-120">Application</span></span>||
| <span data-ttu-id="ec60d-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="ec60d-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="ec60d-122">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec60d-122">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="ec60d-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="ec60d-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="ec60d-124">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec60d-124">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec60d-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec60d-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="ec60d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec60d-126">Request headers</span></span>
|<span data-ttu-id="ec60d-127">标头</span><span class="sxs-lookup"><span data-stu-id="ec60d-127">Header</span></span>|<span data-ttu-id="ec60d-128">值</span><span class="sxs-lookup"><span data-stu-id="ec60d-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec60d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec60d-129">Authorization</span></span>|<span data-ttu-id="ec60d-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec60d-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec60d-131">接受</span><span class="sxs-lookup"><span data-stu-id="ec60d-131">Accept</span></span>|<span data-ttu-id="ec60d-132">application/json</span><span class="sxs-lookup"><span data-stu-id="ec60d-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec60d-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec60d-133">Request body</span></span>
<span data-ttu-id="ec60d-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec60d-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec60d-135">响应</span><span class="sxs-lookup"><span data-stu-id="ec60d-135">Response</span></span>
<span data-ttu-id="ec60d-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec60d-136">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec60d-137">示例</span><span class="sxs-lookup"><span data-stu-id="ec60d-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec60d-138">请求</span><span class="sxs-lookup"><span data-stu-id="ec60d-138">Request</span></span>
<span data-ttu-id="ec60d-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec60d-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="ec60d-140">响应</span><span class="sxs-lookup"><span data-stu-id="ec60d-140">Response</span></span>
<span data-ttu-id="ec60d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec60d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4684

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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







