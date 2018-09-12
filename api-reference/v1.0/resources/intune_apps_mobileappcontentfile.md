# <a name="mobileappcontentfile-resource-type"></a>mobileAppContentFile 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppContentFiles](../api/intune_apps_mobileappcontentfile_list.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 集合|列出 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的属性和关系。|
|[获取 mobileAppContentFile](../api/intune_apps_mobileappcontentfile_get.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|读取 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的属性和关系。|
|[创建 mobileAppContentFile](../api/intune_apps_mobileappcontentfile_create.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|创建新的 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象。|
|[删除 mobileAppContentFile](../api/intune_apps_mobileappcontentfile_delete.md)|无|删除 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)。|
|[更新 mobileAppContentFile](../api/intune_apps_mobileappcontentfile_update.md)|[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|更新 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的属性。|
|[commit 操作](../api/intune_apps_mobileappcontentfile_commit.md)|无|提交给定应用的文件。|
|[renewUpload 操作](../api/intune_apps_mobileappcontentfile_renewupload.md)|无|续订应用程序文件上传的 SAS URI。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|azureStorageUri|字符串|Azure 存储 URI。|
|isCommitted|布尔|指示文件是否已提交的值。|
|id|字符串|文件 ID。|
|createdDateTime|DateTimeOffset|创建文件的时间。|
|name|字符串|文件名称。|
|size|Int64|加密前的文件大小。|
|sizeEncrypted|Int64|加密后的文件大小。|
|azureStorageUriExpirationDateTime|DateTimeOffset|Azure 存储 URI 的到期时间。|
|manifest|Binary|清单信息。|
|uploadState|[mobileAppContentFileUploadState](../resources/intune_apps_mobileappcontentfileuploadstate.md)|当前上传请求的状态。可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String"
}
```








