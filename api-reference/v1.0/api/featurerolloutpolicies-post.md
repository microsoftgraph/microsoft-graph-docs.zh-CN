---
title: 创建 featureRolloutPolicy
description: 创建新的 featureRolloutPolicy 对象。
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0a88d66594d9fa345c54a999f6452a7a287d0b08
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964671"
---
# <a name="create-featurerolloutpolicy"></a>创建 featureRolloutPolicy

命名空间：microsoft.graph

创建新的 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /policies/featureRolloutPolicies
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。 必需 |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象的 JSON 表示形式。

下表显示创建 [featureRolloutPolicy](../resources/featurerolloutpolicy.md)时所需的属性。

| 参数 | 类型 | 说明|
|:---------------|:--------|:----------|
|displayName |string |此功能显示名称策略的部署策略。|
|功能 |stagedFeatureName |将使用此策略推出的功能。|
|isEnabled |string |指示是否启用功能推出。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和一 `201 Created` 个新的 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_featurerolloutpolicy_from_directory"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/featureRolloutPolicies
Content-type: application/json

{
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
  "displayName": "PassthroughAuthentication rollout policy",
  "description": "PassthroughAuthentication rollout policy",
  "feature": "passthroughAuthentication",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


