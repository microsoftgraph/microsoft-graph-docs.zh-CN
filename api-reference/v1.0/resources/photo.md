# <a name="photo-resource-type"></a>照片资源类型

**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1024,
  "exposureNumerator": 1024,
  "fNumber": 1024,
  "focalLength": 1024,
  "iso": 1024,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>属性
| 属性                | 类型                      | 说明                                                     |
|:------------------------|:--------------------------|:----------------------------------------------------------------|
| **takenDateTime**       | DateTimeOffset            | 表示照片拍摄的时间和日期。只读。               |
| **cameraMake**          | String                    | 相机制造商。只读。                                            |
| **cameraModel**         | String                    | 相机型号。只读。                                                   |
| **fNumber**             | Double                    | 相机的 F-stop 值。只读。                               |
| **exposureDenominator** | Int32                     | 相机的曝光时间分数的分母。只读。 |
| **exposureNumerator**   | Int32                     | 相机的曝光时间分数的分子。只读。   |
| **focalLength**         | Double                    | 相机的焦距。只读。                               |
| **iso**                 | Int32                     | 相机的 ISO 值。只读。                                  |

## <a name="remarks"></a>注解
OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。

有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "photo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
