# <a name="list-windowsinformationprotections"></a><span data-ttu-id="1ae34-101">列出 windowsInformationProtections</span><span class="sxs-lookup"><span data-stu-id="1ae34-101">List windowsInformationProtections</span></span>

> <span data-ttu-id="1ae34-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1ae34-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ae34-103">列出 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ae34-103">List properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ae34-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1ae34-104">Prerequisites</span></span>
<span data-ttu-id="1ae34-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1ae34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1ae34-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ae34-107">Permission type</span></span>|<span data-ttu-id="1ae34-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1ae34-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ae34-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ae34-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1ae34-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ae34-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1ae34-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ae34-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ae34-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ae34-112">Not supported.</span></span>|
|<span data-ttu-id="1ae34-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1ae34-113">Application</span></span>|<span data-ttu-id="1ae34-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ae34-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ae34-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ae34-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="1ae34-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ae34-116">Request headers</span></span>
|<span data-ttu-id="1ae34-117">标头</span><span class="sxs-lookup"><span data-stu-id="1ae34-117">Header</span></span>|<span data-ttu-id="1ae34-118">值</span><span class="sxs-lookup"><span data-stu-id="1ae34-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ae34-119">授权</span><span class="sxs-lookup"><span data-stu-id="1ae34-119">Authorization</span></span>|<span data-ttu-id="1ae34-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1ae34-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ae34-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1ae34-121">Accept</span></span>|<span data-ttu-id="1ae34-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1ae34-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ae34-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1ae34-123">Request body</span></span>
<span data-ttu-id="1ae34-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1ae34-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ae34-125">响应</span><span class="sxs-lookup"><span data-stu-id="1ae34-125">Response</span></span>
<span data-ttu-id="1ae34-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1ae34-126">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ae34-127">示例</span><span class="sxs-lookup"><span data-stu-id="1ae34-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ae34-128">请求</span><span class="sxs-lookup"><span data-stu-id="1ae34-128">Request</span></span>
<span data-ttu-id="1ae34-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1ae34-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="1ae34-130">响应</span><span class="sxs-lookup"><span data-stu-id="1ae34-130">Response</span></span>
<span data-ttu-id="1ae34-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1ae34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4598

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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








