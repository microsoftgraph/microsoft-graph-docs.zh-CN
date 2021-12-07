---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 22b825a04b1679385aa0cf14c6421a820b312941
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61321790"
---
# <a name="cloudpcdeviceimage-resource-type"></a>cloudPcDeviceImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑上的图像资源。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceImages](../api/virtualendpoint-list-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。|
|[获取 cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|读取 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcdeviceimage.md) 关系。|
|[创建 cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[删除 cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|无|删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合|获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。|
|[重新加载 cloudPcDeviceImage](../api/cloudpcdeviceimage-reupload.md)|无|重新加载 [无法上载的 cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑上的图像资源的唯一标识符。 只读。|
|sourceImageResourceId|String|Azure 上的源图像资源的 ID。 所需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。|
|displayName|String|图像显示名称。|
|version|String|图像版本。 例如：0.0.1、1.5.13。|
|osBuildNumber|String|映像的操作系统生成版本。 例如：1909。|
|operatingSystem|String|映像的操作系统。 例如：Windows 10 企业版。|
|lastModifiedDateTime|DateTimeOffset|上次修改图像的数据和时间。 时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。 例如，2014 年 1 月 1 日午夜 UTC 显示为"2014-01-01T00：00：00Z"。|
|状态|cloudPcDeviceImageStatus|云电脑上映像的状态。 可取值为：`pending`、`ready`、`failed`。|
|statusDetails|cloudPcDeviceImageStatusDetails|图像状态的详细信息，指示上传失败的原因（如果适用）。 可能的值是 `internalServerError` `sourceImageNotFound` `osVersionNotSupported` ：、、、 `sourceImageInvalid` 和 `sourceImageNotGeneralized` 。|

### <a name="cloudpcdeviceimagestatus-values"></a>cloudPcDeviceImageStatus 值

|成员|说明|
|:---|:---|
|pending|图像上载正在进行中。|
|ready|该映像已准备好在云 PC 上使用。|
|failed|无法上载图像。 |

### <a name="cloudpcdeviceimagestatusdetails-values"></a>cloudPcDeviceImageStatusDetails 值

|成员|说明|
|:---|:---|
|internalServerError|处理映像时出现内部服务器错误。|
|sourceImageNotFound|无法访问或找不到源图像。|
|osVersionNotSupported| 不支持操作系统版本。|
|sourceImageInvalid|源映像用于无效虚拟机Windows虚拟机。|
|sourceImageNotGeneralized|上载的图像尚未通用化。 运行 sysprep/generalize 命令后重新加载映像。 若要了解详细信息，请参阅在创建映像之前通过通用 [化 VM 删除计算机特定信息](/azure/virtual-machines/generalize)。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

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
