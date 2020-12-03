---
title: cloudPcDeviceImage 资源类型
description: 表示云电脑上的图像资源。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 782704beabce8131beb1f5c096d0e35a5a44ca3e
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563842"
---
# <a name="cloudpcdeviceimage-resource-type"></a>cloudPcDeviceImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑上的图像资源。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceImages](../api/virtualendpoint-list-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|列出 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。|
|[获取 cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|读取 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。|
|[创建 cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[删除 cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|无|删除 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|[cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 集合|获取 [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑上的图像资源的唯一标识符。 只读。|
|sourceImageResourceId|String|Azure 上的源图像资源的 ID。 必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}"。|
|displayName|String|图像的显示名称。|
|version|String|图像版本。 例如：0.0.1、1.5.13。|
|osBuildNumber|String|图像的 OS 内部版本。 例如：1909。|
|operatingSystem|String|图像的操作系统。 例如： Windows 10 企业版。|
|lastModifiedDateTime|DateTimeOffset|上次修改图像的数据和时间。 时间以 ISO 8601 格式和协调世界时 (UTC) 时间显示。 例如，2014年1月1日午夜 UTC 显示为 "2014-01-01T00：00： 00Z"。|
|status|cloudPcDeviceImageStatus|云电脑上的映像的状态。 可能的状态包括 "上载挂起"、"上载时失败" 或 "就绪" 可供使用。 可取值为：`pending`、`ready`、`failed`。|
|statusDetails|cloudPcDeviceImageStatusDetails|图像状态的详细信息，用于指示上载失败的原因（如果适用）。 可取值为：`internalServerError`、`sourceImageNotFound`。|

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
