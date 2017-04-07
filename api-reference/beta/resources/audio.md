# <a name="audio-resource-type"></a>音频资源类型

**音频**资源将与音频相关的属性分组到一个单一结构。

如果 [**DriveItem**](driveitem.md) 具有一个非 null **音频** facet，则该项表示一个音频文件。通过从文件中提取元数据来填充**音频**资源的属性。 

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.audio"
}-->
```json
{
  "album": "string",
  "albumArtist": "string",
  "artist": "string",
  "bitrate": 1024,
  "composers": "string",
  "copyright": "string",
  "disc": 1024,
  "discCount": 1024,
  "duration": 1024,
  "genre": "string",
  "hasDrm": true,
  "isVariableBitrate": true,
  "title": "string",
  "track": 1024,
  "trackCount": 1024,
  "year": 1024
}
```

## <a name="properties"></a>属性

| 属性          | 类型    | 说明                                                          |
|:------------------|:--------|:---------------------------------------------------------------------|
| album             | string  | 此音频文件的专辑标题。                          |
| albumArtist       | string  | 此音频文件的专辑上指定的艺术家。                    |
| artist            | string  | 音频文件的表演艺术家。                            |
| bitrate           | string  | 以 kbps 表示的比特率。                                           |
| composers         | string  | 音频文件的作曲者姓名。                          |
| copyright         | string  | 音频文件的版权信息。                            |
| disc              | 数字  | 此音频文件源自的光盘编号。                    |
| discCount         | 数字  | 此专辑中的光盘总数。                             |
| duration          | 数字  | 音频文件的持续时间，以毫秒表示                |
| genre             | string  | 此音频文件的流派。                                        |
| hasDrm            | boolean | 指示文件是否受数字版权管理的保护。   |
| isVariableBitrate | boolean | 指示文件是否已通过可变比特率编码。            |
| title             | string  | 音频文件的标题。                                         |
| track             | 数字  | 此音频文件的原始光盘上的曲目数。    |
| trackCount        | 数字  | 此音频文件的原始光盘上的曲目总数。 |
| year              | 数字  | 录制音频文件的年份。                                |

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audio resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->