---
title: 克隆团队
description: 创建团队的副本。 此操作还会创建相应组的副本。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5368e2128a5c4010f218639574104a09371636ee
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335693"
---
# <a name="clone-a-team"></a>克隆团队

命名空间：microsoft.graph



创建[团队](../resources/team.md)的副本。 此操作还会创建相应[组](../resources/group.md)的副本。
您可以指定要克隆的团队部分：

- **应用**-复制团队中安装的 Microsoft 团队应用。 
- **频道**–复制通道结构（而不是通道中的邮件）。
- **members** –复制组的成员和所有者。
- **设置**–复制团队内的所有设置以及关键组设置。
- **选项卡**–复制频道中的选项卡。

当选项卡被克隆时，它们将被置于未配置状态--它们将显示在 Microsoft 团队中的选项卡栏上，在第一次打开它们时，您将完成配置屏幕。 （如果打开该选项卡的用户没有配置应用的权限，他们将看到一条消息，说明该选项卡尚未配置。）

克隆是一项长时间运行的操作。
在 POST 克隆返回之后，您需要获取[操作](../resources/teamsasyncoperation.md)，以查看它是 "正在运行" 还是 "已成功" 或 "失败"。 您应继续获取，直到状态不为 "正在运行"。 建议的获取延迟为5秒。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Group.ReadWrite.All、Directory.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序                            | Group.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文

| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|classification|String （可选）|描述组的分类（如低、中或高业务影响）。 如果未指定分类，则将从原始团队/组复制分类。|
|说明|String （可选）|可选的组说明。 如果未指定此属性，则它将保留为空。|
|displayName|String|组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。|
|mailNickname|String|组的邮件别名，在组织中是唯一的。 创建组时必须指定此属性。 支持 $filter。 如果未指定此属性，则将从 displayName 计算。 已知问题：此属性当前被忽略。|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |要克隆的部分的逗号分隔列表。 法律部门是 "应用、选项卡、设置、通道、成员"。|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) （可选）| 指定组的可见性。 可能的值为： **Private**、 **Public**。 如果未指定可见性，将从原始团队/组复制可见性。 如果克隆的团队是**educationClass**团队，则忽略 visibility 参数，新组的可见性将设置为 HiddenMembership。|

## <a name="response"></a>响应

如果成功，此方法将返回一个 `202 Accepted` 位置为的响应代码：标头，指向[操作](../resources/teamsasyncoperation.md)资源。
操作完成后，操作资源将告知您创建的团队的 id。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clone_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clone-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clone-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clone-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clone-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
