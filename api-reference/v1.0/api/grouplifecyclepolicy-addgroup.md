---
title: 'groupLifecyclePolicy: addGroup'
description: 将组添加到生命周期策略。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2f2c8798dcff6cf0883453512b3c322596208d5e
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589168"
---
# <a name="grouplifecyclepolicy-addgroup"></a>groupLifecyclePolicy: addGroup

命名空间：microsoft.graph

将特定组添加到生命周期策略。 只有在 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 的 **managedGroupTypes** 属性设置为 时，此操作才将组生命周期策略限制到一组`Selected`组。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Directory.ReadWrite.All                     |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| Application                            | Directory.ReadWrite.All                     |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /groupLifecyclePolicies/{id}/addGroup
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json          |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数 | 类型   | 说明                                       |
| :-------- | :----- | :------------------------------------------------ |
| groupId   | String | 要添加到策略的组的标识符。 |

当 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) `Selected`的 **managedGroupTypes** 属性设置为 时，您最多可以将 500 个组添加到列表中。 如果需要添加 500 多个组，[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 的 **managedGroupTypes** 属性必须设置为 `All`。

每个请求只能添加一个组。

## <a name="response"></a>响应

如果成功，此方法返回 `200 OK` 响应代码。 如果组已添加到策略，响应 `true` 正文中将返回一个值。 否则， `false` 在响应正文中返回值。

## <a name="example"></a>示例

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "grouplifecyclepolicy_addgroup"
} -->

```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}/addGroup
Content-type: application/json

{
  "groupId": "ffffffff-ffff-ffff-ffff-ffffffffffff"
}
```

#### <a name="response"></a>响应

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy: addgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
