---
title: unsupportedDeviceConfigurationDetail 资源类型
description: 为什么说实体是不受支持的说明。
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344049"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>unsupportedDeviceConfigurationDetail 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

为什么说实体是不受支持的说明。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|message|字符串|解释 entity 为什么不受支持的一条消息。|
|propertyName|字符串|如果邮件与原始实体，则该属性的名称中的特定属性。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





