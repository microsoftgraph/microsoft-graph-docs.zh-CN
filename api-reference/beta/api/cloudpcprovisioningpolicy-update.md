---
title: 更新 cloudPcProvisioningPolicy
description: 更新 cloudPcProvisioningPolicy 对象的属性。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 25957fe267af7e33b82d5596ddfdfbb102dc0716
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447084"
---
# <a name="update-cloudpcprovisioningpolicy"></a>更新 cloudPcProvisioningPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [cloudPcProvisioningPolicy 对象的](../resources/cloudpcprovisioningpolicy.md) 属性。

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
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明                |
| :------------ | :------------------------  |
| Authorization | Bearer {token}。必需。  |
| Content-Type  | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的 JSON 表示形式。

下表显示了可针对 [cloudPcProvisioningPolicy 更新的](../resources/cloudpcprovisioningpolicy.md)属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|预配策略的显示名称。 |
|说明|String|预配策略说明。|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|指定云电脑如何加入 Azure Active Directory。|
|onPremisesConnectionId|String|cloudPcOnPremisesConnection 的 ID。 若要确保云电脑具有网络连接且它们已加入域，请选择与云电脑服务验证的虚拟网络的连接。|
|imageId|String|要在云电脑上预配的 OS 映像的 ID。 库类型图像的格式为：{publisher_offer_sku}。 每个参数支持的值如下所示： <ul><li>发布者：Microsoftwindowsdesktop。</li> <li>offer： windows-ent-cpc.</li> <li>sku： 21h1-ent-cpc-m365， 21h1-ent-cpc-os、20h2-ent-cpc-m365、20h2-ent-cpc-os、20h1-ent-cpc-m365、20h1-ent-cpc-os、19h2-ent-cpc-m365 和 19h2-ent-cpc-os。</li></ul>|
|imageDisplayName|String|要预配的 OS 映像的显示名称。|
|imageType|cloudPcProvisioningPolicyImageType|要在云电脑上预配) 自定义或库 (OS 映像的类型。 可取值为：`gallery`、`custom`。|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|具有此预配策略的预配云电脑的 Windows 操作系统设置，例如操作系统语言设置。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_provisioningpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "HR provisioning policy",
  "description": "Provisioning policy for India HR employees",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom",
  "windowsSettings": {
    "language": "en-US"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-provisioningpolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-provisioningpolicy-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
}
-->
``` http
HTTP/1.1 204 No Content
```
