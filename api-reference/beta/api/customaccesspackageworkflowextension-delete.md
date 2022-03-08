---
title: 删除 customAccessPackageWorkflowExtension
description: 删除 customAccessPackageWorkflowExtension 对象。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 19178d6d1620b5c21fcc150b3b1699f25362575d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338356"
---
# <a name="delete-customaccesspackageworkflowextension"></a>删除 customAccessPackageWorkflowExtension
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md) 对象。 必须先从任何关联的策略中删除自定义工作流 [扩展，然后才能](../resources/accesspackageassignmentpolicy.md) 删除该扩展。 按照以下步骤从任何关联的策略中删除自定义工作流扩展：
1. 首先通过调用 [Get accessPackageAssignmentPolicies](accesspackageassignmentpolicy-get.md) 操作并追加 `?$expand=accessPackage($expand=accessPackageCatalog)` 到查询来检索 accessPackageCatalogId。 例如，`https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies?$expand=accessPackage($expand=accessPackageCatalog)`。
2. 使用访问包目录 ID，并运行 [LIST customAccessPackageWorkflowExtensions 操作检索要删除的 customAccessPackageWorkflowExtension](accesspackagecatalog-list-customaccesspackageworkflowextensions.md) 对象的 ID。
3. 调用 [Update accessPackageAssignmentPolicy](accesspackageassignmentpolicy-update.md) 操作以从策略中删除自定义工作流扩展对象。 有关示例，请参阅 [示例 2：从策略中删除 customExtensionHandlers](accesspackageassignmentpolicy-update.md#example-2-remove-the-customextensionhandlers-from-a-policy)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|EntitlementManagement.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|EntitlementManagement.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/{catalogId}/customAccessPackageWorkflowExtensions/{customAccessPackageWorkflowExtensionId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_customaccesspackageworkflowextension"
}
-->
``` http
DELETE /identityGovernance/entitlementManagement/accessPackageCatalogs/32efb28c-9a7a-446c-986b-ca6528c6669d/customAccessPackageWorkflowExtensions/98ffaec5-ae8e-4902-a434-5ffc5d3d3cd0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-customaccesspackageworkflowextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-customaccesspackageworkflowextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-customaccesspackageworkflowextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-customaccesspackageworkflowextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-customaccesspackageworkflowextension-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-customaccesspackageworkflowextension-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Response
```
