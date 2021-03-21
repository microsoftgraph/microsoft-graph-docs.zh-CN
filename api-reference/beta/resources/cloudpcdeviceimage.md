---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: d4a88bb4d826ead30d1d739e696dec76df5cbb2f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957063"
---
# <a name="cloudpcdeviceimage-resource-type"></a>cloudPcDeviceImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑上的图像资源。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceImages](../api/virtualendpoint-list-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。|
|[获取 cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|读取 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。|
|[创建 cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[删除 cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|无|删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合|获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑上的图像资源的唯一标识符。 只读。|
|sourceImageResourceId|String|Azure 上的源图像资源的 ID。 所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。|
|displayName|String|图像的显示名称。|
|version|String|图像版本。 例如：0.0.1、1.5.13。|
|osBuildNumber|String|映像的操作系统生成版本。 例如：1909。|
|operatingSystem|String|映像的操作系统。 例如：Windows 10 企业版。|
|lastModifiedDateTime|DateTimeOffset|上次修改图像的数据和时间。 时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。 例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。|
|状态|cloudPcDeviceImageStatus|云电脑上映像的状态。 可取值为：`pending`、`ready`、`failed`。|
|statusDetails|cloudPcDeviceImageStatusDetails|图像状态的详细信息，指示上传失败的原因（如果适用）。 可取值为：`internalServerError`、`sourceImageNotFound`。|

### <a name="cloudpcdeviceimagestatus-values"></a>cloudPcDeviceImageStatus 值

|成员|说明|
|:---|:---|
|pending|图像上载正在进行中。|
|ready|该映像已准备好在云电脑使用。|
|failed|无法上载图像。 |

### <a name="cloudpcdeviceimagestatusdetails-values"></a>cloudPcDeviceImageStatusDetails 值

|成员|说明|
|:---|:---|
|internalServerError|处理映像时出现内部服务器错误。|
|sourceImageNotFound|无法访问或找不到源图像。|
|osVersionNotSupported| 不支持操作系统版本。|
|sourceImageInvalid|源映像用于无效 Windows VM。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
