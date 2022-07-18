---
title: Create customAccessPackageWorkflowExtensions
description: 创建新的 customAccessPackageWorkflowExtension 对象。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 95939d13b49bb599cb1f43661b5c9398e79d3710
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338200"
---
# <a name="create-customaccesspackageworkflowextensions"></a>Create customAccessPackageWorkflowExtensions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象并将其添加到现有 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象。  

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/customAccessPackageWorkflowExtensions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象的 JSON 表示形式。

可以在创建自定义 **AccessPackageWorkflowExtension时指定以下属性**。

|属性|类型|说明|
|:---|:---|:---|
|说明|String|customAccessPackageWorkflowExtension 对象的说明。|
|displayName|字符串|customAccessPackageWorkflowExtension 的显示名称。|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|用于配置终结点以调用逻辑应用的工作流的类型和详细信息。|  
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|用于保护对逻辑应用的 API 调用的配置。 例如，使用 OAuth 客户端凭据流。|



## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_customaccesspackageworkflowextension_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/32efb28c-9a7a-446c-986b-ca6528c6669d/customAccessPackageWorkflowExtensions
Content-Type: application/json

{ 
    "displayName": "test_action_0124", 
    "description": "this is for graph testing only", 
    "endpointConfiguration": { 
        "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration", 
        "subscriptionId": "38ab2ccc-3747-4567-b36b-9478f5602f0d", 
        "resourceGroupName": "EMLogicApp", 
        "logicAppWorkflowName": "customextension_test" 
    }, 
    "authenticationConfiguration": { 
        "@odata.type": "#microsoft.graph.azureAdTokenAuthentication", 
        "resourceId": "f604bd15-f785-4309-ad7c-6fad18ddb6cb" 
    } 
} 
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-customaccesspackageworkflowextension-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-customaccesspackageworkflowextension-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-customaccesspackageworkflowextension-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-customaccesspackageworkflowextension-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-customaccesspackageworkflowextension-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-customaccesspackageworkflowextension-from--powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customAccessPackageWorkflowExtension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{ 
    "id": "98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0", 
    "displayName": "test_action_0124",
    "description": "this is for graph testing only", 
    "createdDateTime": "2022-01-24T21:48:57.1483656Z", 
    "lastModifiedDateTime": "2022-01-24T21:48:57.1483656Z", 
    "clientConfiguration": null, 
    "endpointConfiguration": { 
        "@odata.type": "#microsoft.graph.logicAppTriggerEndpointConfiguration", 
        "subscriptionId": "38ab2ccc-3747-4567-b36b-9478f5602f0d", 
        "resourceGroupName": "EMLogicApp", 
        "logicAppWorkflowName": "customextension_test" 
    },
    "authenticationConfiguration": { 
        "@odata.type": "#microsoft.graph.azureAdTokenAuthentication", 
        "resourceId": "f604bd15-f785-4309-ad7c-6fad18ddb6cb" 
    } 
} 
```

