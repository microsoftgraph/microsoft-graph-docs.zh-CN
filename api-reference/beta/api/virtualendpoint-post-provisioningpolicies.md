---
title: 创建 cloudPcProvisioningPolicy
description: 创建新的云电脑预配策略。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 60422e27d69ddc23faa3708bc4d625a420d0c2c3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446159"
---
# <a name="create-cloudpcprovisioningpolicy"></a>创建 cloudPcProvisioningPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|CloudPC.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                |
| :------------ | :------------------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的 JSON 表示形式。

下表显示了创建 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|预配策略的显示名称。|
|说明|String|预配策略说明。|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|指定云电脑如何加入 Azure Active Directory。|
|onPremisesConnectionId|String|cloudPcOnPremisesConnection 的 ID。 若要确保云电脑具有网络连接且它们已加入域，请选择与云电脑服务验证的虚拟网络的连接。|
|imageId|String|要在云电脑上预配的 OS 映像的 ID。 库类型图像的格式为：{publisher_offer_sku}。 每个参数支持的值如下所示：<ul><li>发布者：Microsoftwindowsdesktop。</li> <li>offer： windows-ent-cpc.</li> <li>sku： 21h1-ent-cpc-m365， 21h1-ent-cpc-os、20h2-ent-cpc-m365、20h2-ent-cpc-os、20h1-ent-cpc-m365、20h1-ent-cpc-os、19h2-ent-cpc-m365 和 19h2-ent-cpc-os。</li></ul>|
|imageDisplayName|String|要预配的 OS 映像的显示名称。|
|imageType|cloudPcProvisioningPolicyImageType|要在云电脑上预配) 自定义或库 (OS 映像的类型。 可取值为：`gallery`、`custom`。|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|为此预配策略创建云电脑时要配置的特定 Windows 设置。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
    "description": "Description value",
    "displayName": "Display Name value",
    "domainJoinConfiguration": {
        "domainJoinType": "hybridAzureADJoin",
        "onPremisesConnectionId": "16ee6c71-fc10-438b-88ac-daa1ccafffff"
    },
    "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
    "imageDisplayName": "Windows-10 19h1-evd",
    "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
    "imageType":"gallery",
    "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
    "windowsSettings": {
        "language": "en-US"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "description": "Description value",
  "displayName": "Display Name value",
  "domainJoinConfiguration": {
      "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
      "type": "hybridAzureADJoin"
  },
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "imageDisplayName": "Windows-10 19h1-evd",
  "imageId": "MicrosoftWindowsDesktop_Windows-10_19h1-evd",
  "imageType":"gallery",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "windowsSettings": {
    "language": "en-US"
  },
  "managedBy": "windows365"
}
```
