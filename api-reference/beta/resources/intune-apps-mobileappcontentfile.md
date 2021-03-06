---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5004a7b5d7ee1c38e559c41a86155cd89506af3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281010"
---
# <a name="mobileappcontentfile-resource-type"></a>mobileAppContentFile 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[List mobileAppContentFiles](../api/intune-apps-mobileappcontentfile-list.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合|列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。|
|[Get mobileAppContentFile](../api/intune-apps-mobileappcontentfile-get.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。|
|[Create mobileAppContentFile](../api/intune-apps-mobileappcontentfile-create.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。|
|[Delete mobileAppContentFile](../api/intune-apps-mobileappcontentfile-delete.md)|无|删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。|
|[Update mobileAppContentFile](../api/intune-apps-mobileappcontentfile-update.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。|
|[commit 操作](../api/intune-apps-mobileappcontentfile-commit.md)|无|提交给定应用的文件。|
|[renewUpload 操作](../api/intune-apps-mobileappcontentfile-renewupload.md)|无|续订应用程序文件上传的 SAS URI。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|azureStorageUri|String|Azure 存储 URI。|
|isCommitted|Boolean|指示文件是否已提交的值。|
|id|字符串|文件 ID。|
|createdDateTime|DateTimeOffset|创建文件的时间。|
|name|字符串|文件名称。|
|size|Int64|加密前的文件大小。|
|sizeEncrypted|Int64|加密后的文件大小。|
|azureStorageUriExpirationDateTime|DateTimeOffset|Azure 存储 URI 的到期时间。|
|manifest|Binary|清单信息。|
|uploadState|[mobileAppContentFileUploadState](../resources/intune-apps-mobileappcontentfileuploadstate.md)|当前上传请求的状态。 可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。|
|isFrameworkFile|Boolean|一个指示文件是否为框架文件的值。|
|isDependency|Boolean|内容文件是否依赖于主要内容文件。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
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
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```




