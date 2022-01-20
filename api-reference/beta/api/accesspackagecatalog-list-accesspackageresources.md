---
title: 列出 accessPackageResources
description: 检索 accesspackageresource 对象的列表。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6948b7ca0d7c8b9b4c3d47221516cc4ea79d7992
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091106"
---
# <a name="list-accesspackageresources"></a>列出 accessPackageResources

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[accessPackageCatalog](../resources/accesspackagecatalog.md)中检索[accessPackageResource](../resources/accesspackageresource.md)对象的列表。  若要请求添加或删除 [accessPackageResource](../resources/accesspackageresource.md)，请使用 [create accessPackageResourceRequest](entitlementmanagement-post-accesspackageresourcerequests.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。 例如，若要检索每个资源的访问包资源范围和环境，请包括在 `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` 查询中。 若要检索资源的可用角色，请包含 `$expand=accessPackageResourceRoles` 。 若要仅检索应用程序的资源，而不是检索组或网站的资源，请 `$filter=resourceType eq 'Application'` 包括在查询中。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageResource](../resources/accesspackageresource.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面是一个请求示例，使用筛选器选择特定类型的资源并 `$expand` 返回每个资源的资源范围。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources?$filter=resourceType eq 'Application'&$expand=accessPackageResourceScopes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accesspackageresources-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-accesspackageresources-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
      "accessPackageResourceScopes": [
          {
              "id": "452d78a7-69a5-482d-a82f-859a5169c55e",
              "displayName": "Root",
              "description": "Root Scope",
              "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
              "originSystem": "AadApplication",
              "isRootScope": true
          }
      ],
      "attributes": [
          {
              "id": "4f28e638-93de-4152-b631-2135da14c94a",
              "attributeName": "country",
              "attributeDefaultValue": null,
              "isEditable": true,
              "isPersistedOnAssignmentRemoval": false,
              "attributeSource": {
                  "@odata.type": "#microsoft.graph.resourceAttributeQuestion",
                  "question": {
                      "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
                      "id": "6c797e12-e608-4ac9-90da-a8f18df37a94",
                      "isRequired": false,
                      "isAnswerEditable": null,
                      "sequence": 0,
                      "allowsMultipleSelection": false,
                      "text": {
                          "defaultText": "Enter your country",
                          "localizedTexts": []
                      },
                      "choices": [
                          {
                              "actualValue": "USA",
                              "displayValue": {
                                  "defaultText": "USA",
                                  "localizedTexts": [
                                      {
                                          "text": "USA",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          },
                          {
                              "actualValue": "Canada",
                              "displayValue": {
                                  "defaultText": "Canada",
                                  "localizedTexts": [
                                      {
                                          "text": "Canada",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          },
                          {
                              "actualValue": "India",
                              "displayValue": {
                                  "defaultText": "India",
                                  "localizedTexts": [
                                      {
                                          "text": "English",
                                          "languageCode": "en-US"
                                      }
                                  ]
                              }
                          }
                      ]
                  }
              },
              "attributeDestination": {
                  "@odata.type": "#microsoft.graph.userDirectoryAttributeStore"
              }
          }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
