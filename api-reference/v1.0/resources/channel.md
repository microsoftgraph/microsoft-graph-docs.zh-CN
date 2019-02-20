# <a name="channel-resource-type"></a>通道资源类型



频道是[团队](../resources/team.md)中的邮件的集合。 通道表示一个主题，因此讨论，团队中的逻辑隔离。 示例可以是"星期五团队可边午餐"通道和"体系结构讨论"通道。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列表通道](../api/channel_list.md) | [通道](channel.md)集合 | 此团队中获取通道的列表。|
|[创建通道](../api/channel_post.md) | [通道](channel.md) | 创建新的通道通过包括的显示名称和说明。|
|[获取通道](../api/channel_get.md) | [通道](channel.md) | 读取属性和该频道的关系。|
|[更新通道](../api/channel_patch.md) | [通道](channel.md) | 更新该频道的属性。|
|[删除通道](../api/channel_delete.md) | 无 | 删除通道。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|字符串|通道的可选文字说明。|
|displayName|字符串|通道名称将显示于 Microsoft 团队中的用户。|
|id|字符串|通道的唯一标识符。 只读。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|选项卡|[teamsTab](../resources/teamstab.md)集合|在进入频道的所有选项卡的集合。 导航属性。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "chatthreads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "channel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
