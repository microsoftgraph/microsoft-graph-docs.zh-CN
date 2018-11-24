# <a name="clone-a-team"></a>克隆团队



创建[团队](../resources/team.md)的副本。 此操作还将创建相应的[组](../resources/group.md)的副本。
您可以指定团队要克隆哪些的部分：

- **应用程序**-副本的 Microsoft 团队的团队中安装的应用程序。 
- **通道**– 将复制的通道结构 （但不是在进入频道的消息）。
- **成员**– 将复制的成员和组的所有者。
- **设置**– 将复制的团队，以及关键组设置中的所有设置。
- **选项卡**– 副本通道中的选项卡。

选项卡克隆时，他们将放在未配置状态--Microsoft 团队中的选项卡栏上显示和首次打开它们，您将通过配置屏幕。 （如果打开选项卡的人员没有配置应用程序的权限，他们将看到一条消息，说明尚未已配置选项卡）。

克隆是长时间运行的操作。
POST 克隆返回后，您需要获取[操作](../resources/teamsasyncoperation.md)以查看是否"运行"或"成功"或"失败"。 您应继续 GET 之前状态未"运行"。 获取之间的建议的延迟为 5 秒。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | Group.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序                            | Group.ReadWrite.All |

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
|Classification|字符串 （可选）|介绍组 （如低、 中等或高的业务影响） 的分类。 如果未指定分类，将从原始团队组复制的分类。|
|说明|字符串 （可选）|可选的组说明。 如果未指定此属性，它将为空。|
|displayName|字符串|组的显示名称。此属性是在创建组时所必需的，并且在更新过程中不能清除。支持 $filter 和 $orderby。|
|mailNickname|字符串|邮件的组中，组织中唯一的别名。 创建组后，必须指定此属性。 支持 $filter。 如果未指定此属性，将从 displayName 计算。 已知问题： 当前忽略此属性。|
|partsToClone| [clonableTeamParts](../resources/clonableteamparts.md) |要克隆的部分以逗号分隔列表。 法律部件是"应用程序、 选项卡、 设置、 通道、 成员"。|
|visibility|[teamVisibilityType](../resources/teamVisibilityType.md)（可选）| 指定组的可见性。 可能的值为：**专用**的**公共**。 如果未指定可见性，则将从原始团队组复制可见性。 如果正在克隆团队**educationClass**团队、 可见性参数将被忽略，并将被新组的可见性设置为 HiddenMembership。|

## <a name="response"></a>响应

如果成功，则此方法将返回`202 Accepted`与某个位置的响应代码： 指向[操作](../resources/teamsasyncoperation.md)资源的标头。
完成该操作后，操作资源会告诉您创建的团队的 id。

## <a name="example"></a>示例
#### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "ignored",
  "name": "create_team"
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

#### <a name="response"></a>响应
下面展示了示例响应。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
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
