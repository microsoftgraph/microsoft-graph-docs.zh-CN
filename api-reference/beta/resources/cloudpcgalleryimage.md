---
title: cloudPcGalleryImage 资源类型
description: 表示当前组织的库图像资源。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 7c539af9b8a31000af06cb88de594d80c4ea5eb5
ms.sourcegitcommit: c00c61ce35a6f204a9907aa6f2644ea7a86a5b6e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2021
ms.locfileid: "60805538"
---
# <a name="cloudpcgalleryimage-resource-type"></a>cloudPcGalleryImage 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可用于预配云电脑的当前组织的库图像资源。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[List galleryImages](../api/virtualendpoint-list-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcgalleryimage.md) 集合|列出 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcgalleryimage.md) 关系。|
|[获取 cloudPcGalleryImage](../api/cloudpcgalleryimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcgalleryimage.md)|读取 [cloudPcDeviceImage 对象的属性和](../resources/cloudpcgalleryimage.md) 关系。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|库显示名称的官方图像。 只读。|
|endDate|日期|此图像不再位于长期支持范围内的日期。 云电脑将继续提供短期支持。 只读。|
|expirationDate|日期|图像不再可用的日期。 只读。|
|id|String|云电脑上库图像资源的唯一标识符。 只读。|
|offer|String|库图像的优惠名称。 此值将传递到 Azure，以获取图像资源。 只读。|
|offerDisplayName|String|库图像的官方显示产品/服务名称。 例如，Windows 10 企业版 + 操作系统优化。 只读。|
|发布者|String|库图像的发布者名称。 此值将传递到 Azure，以获取图像资源。 只读。|
|recommendedSku|String|此库映像的建议云电脑 SKU。 只读。|
|sizeInGB|Int32|此图像的大小（以 GB 为单位）。 只读。|
|sku|String|库图像的 SKU 名称。 此值将传递到 Azure，以获取图像资源。 只读。|
|skuDisplayName|String|官方显示库存单元 (SKU) 库图像的名称。 例如，2004。 只读。|
|startDate|日期|图像可用的日期。 只读。|
|status|cloudPcGalleryImageStatus|云电脑上库图像的状态。 可能的值是：`supported`、`supportedWithWarning`、`notSupported`、`unknownFutureValue`。 只读。|

### <a name="cloudpcgalleryimagestatus-values"></a>cloudPcGalleryImageStatus 值

|成员|说明|
|:---|:---|
|支持|库图像处于活动状态，并准备用于预配。|
|supportedWithWarning|库图像已过期，但云电脑将继续支持 6 个月，此后它将不受支持且无法使用。|
|notSupported|库图像已不支持。 |
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcGalleryImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName":"String",
  "offerDisplayName":"String",
  "skuDisplayName":"String",
  "publisher":"String",
  "offer":"String",
  "sku":"String",
  "recommendedSku":"String",
  "status":"String",
  "sizeInGB":"Int32",
  "startDate":"String (Date)",
  "endDate":"String (Date)",
  "expiredDate":"String (Date)"
}
```
