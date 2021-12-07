---
title: microsoftManagedDesktop 资源类型
description: 表示客户能够Microsoft 托管桌面云电脑的托管设备体验的设备的特定设置。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 26eadd11fc46ba794249f1d6f1094a000777b5cf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322757"
---
# <a name="microsoftmanageddesktop-resource-type"></a>microsoftManagedDesktop 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示客户能够Microsoft 托管桌面云电脑的托管设备体验的设备的特定设置。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|个人资料|String|与 365 Microsoft 托管桌面关联的Windows配置文件的名称。|
|type|[microsoftManagedDesktopType](#microsoftmanageddesktoptype-values)|指示预配策略是否启用Microsoft 托管桌面。 它指示在启用预配策略时管理设备的计划类型。 可取值为：`notManaged`、`premiumManaged`、`standardManaged`、`starterManaged`、`unknownFutureValue`。|

### <a name="microsoftmanageddesktoptype-values"></a>microsoftManagedDesktopType 值

|成员|说明|
|:---|:---|
|notManaged|设备不由 Microsoft 托管桌面。|
|premiumManaged|设备由高级Microsoft 托管桌面管理。|
|standardManaged|设备由标准Microsoft 托管桌面管理。|
|starterManaged|设备由初学者Microsoft 托管桌面进行管理。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftManagedDesktop"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.microsoftManagedDesktop",
  "type": "String",
  "profile": "String"
}
```
