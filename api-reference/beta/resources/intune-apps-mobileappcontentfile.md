---
title: mobileAppContentFile 资源类型
description: 包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e9f28ea036bbe73fae8e9e59d8d63ea8916f15d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425678"
---
# <a name="mobileappcontentfile-resource-type"></a>mobileAppContentFile 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含与给定 mobileAppContent 版本关联的单个安装程序文件的属性。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List mobileAppContentFiles](../api/intune-apps-mobileappcontentfile-list.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合|列出 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。|
|[Get mobileAppContentFile](../api/intune-apps-mobileappcontentfile-get.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|读取 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性和关系。|
|[Create mobileAppContentFile](../api/intune-apps-mobileappcontentfile-create.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。|
|[Delete mobileAppContentFile](../api/intune-apps-mobileappcontentfile-delete.md)|无|删除 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)。|
|[Update mobileAppContentFile](../api/intune-apps-mobileappcontentfile-update.md)|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)|更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。|
|[commit 操作](../api/intune-apps-mobileappcontentfile-commit.md)|无|提交给定应用的文件。|
|[renewUpload 操作](../api/intune-apps-mobileappcontentfile-renewupload.md)|无|续订应用程序文件上传的 SAS URI。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|azureStorageUri|String|Azure 存储 URI。|
|isCommitted|Boolean|指示文件是否已提交的值。|
|id|String|文件 ID。|
|createdDateTime|DateTimeOffset|创建文件的时间。|
|name|String|文件名称。|
|size|Int64|加密前的文件大小。|
|sizeEncrypted|Int64|加密后的文件大小。|
|azureStorageUriExpirationDateTime|DateTimeOffset|Azure 存储 URI 的到期时间。|
|manifest|Binary|清单信息。|
|uploadState|[mobileAppContentFileUploadState](../resources/intune-apps-mobileappcontentfileuploadstate.md)|当前上传请求的状态。 可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。|
|isFrameworkFile|Boolean|指示文件是否框架文件的值。|
|isDependency|Boolean|内容的文件是否依赖关系的主要内容文件。|

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




