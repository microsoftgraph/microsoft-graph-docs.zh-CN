# <a name="userinstallstatesummary-resource-type"></a>userInstallStateSummary 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含某个用户的安装状态摘要的属性。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 userInstallStateSummaries](../api/intune_books_userinstallstatesummary_list.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 集合|列出 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 对象的属性和关系。|
|[获取 userInstallStateSummary](../api/intune_books_userinstallstatesummary_get.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|读取 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 对象的属性和关系。|
|[创建 userInstallStateSummary](../api/intune_books_userinstallstatesummary_create.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|创建新的 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 对象。|
|[删除 userInstallStateSummary](../api/intune_books_userinstallstatesummary_delete.md)|无|删除 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)。|
|[更新 userInstallStateSummary](../api/intune_books_userinstallstatesummary_update.md)|[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)|更新 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|实体的键。|
|userName|字符串|用户名。|
|installedDeviceCount|Int32|已安装设备的计数。|
|failedDeviceCount|Int32|已失败设备的计数。|
|notInstalledDeviceCount|Int32|Not installed device count。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceStates|[deviceInstallState](../resources/intune_books_deviceinstallstate.md) 集合|电子书的安装状态。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.userInstallStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "String (identifier)",
  "userName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```



