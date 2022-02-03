---
title: 克隆团队
description: 创建团队副本。 此操作还会创建相应组的副本。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1d11df106e2fde2003ab2f813a1873476f84b567
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347475"
---
# <a name="clone-a-team"></a>克隆团队

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建团队 [副本](../resources/team.md)。 此操作还会创建相应组 [的副本](../resources/group.md)。
可以指定要克隆的团队的哪些部分：

- **应用** - Microsoft Teams团队中安装的应用。 
- **channels** – 将频道结构 (，但不复制频道中) 。
- **members** – 复制组的成员和所有者。
- **settings** - 复制团队内的所有设置以及关键组设置。
- **tabs** – 在频道内复制选项卡。

克隆选项卡时，这些选项卡将进入未配置状态 -它们显示在 Microsoft Teams 中的选项卡栏上，首次打开它们时，你将通过配置屏幕。  (如果打开选项卡的用户没有配置应用的权限，他们会看到一条消息，说明尚未配置选项卡。) 

克隆是一项长时间运行的操作。
POST 克隆返回后，您需要获取 Location： 标头返回[](../resources/teamsasyncoperation.md)的操作，以查看其是否"正在运行"或"成功"或"失败"。 您应该继续 GET，直到状态未"正在运行"。 GET 之间的建议延迟为 5 秒。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Team.Create、Group.ReadWrite.All **、Directory.ReadWrite.All** |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序                            | Team.Create、Group.ReadWrite.All **、Directory.ReadWrite.All** |

> **注意**：标记为 ** 的权限已弃用，不应使用。

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

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|classification|可选 (字符串) |介绍组策略分类 (低、中或高业务影响) 。 此属性的有效值通过基于模板定义创建 [ClassificationList 设置](../resources/directorysetting.md) 值 [进行定义](../resources/directorysettingtemplate.md)。 如果未指定分类，则从原始团队/组复制分类。|
|description|可选 (字符串) |可选的组说明。 如果未指定此属性，则此属性将留空。|
|displayName|String|组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。|
|mailNickname|String|组的邮件别名，在组织中是唯一的。 创建组时必须指定此属性。 支持 $filter。 如果未指定此属性，则从 displayName 计算此属性。 已知问题：此属性当前被忽略。|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |要克隆的部件的逗号分隔列表。 法律部分为"应用、选项卡、设置、频道、成员"。|
|visibility|[teamVisibilityType](../resources/teamvisibilitytype.md) (可选) | 指定组的可见性。 可能的值是： **Private**、 **Public**。 如果未指定可见性，则从原始团队/组复制可见性。 如果要克隆的团队是 **educationClass** 团队，则忽略 visibility 参数，并且新组的可见性将设置为 HiddenMembership。|

## <a name="response"></a>响应

如果成功，此方法将返回包含 `202 Accepted` 指向操作资源的 Location： 标头 [的响应](../resources/teamsasyncoperation.md) 代码。
操作完成后，操作资源将告知你已创建团队的 ID。

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

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/clone-team-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/clone-team-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams({id})/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


