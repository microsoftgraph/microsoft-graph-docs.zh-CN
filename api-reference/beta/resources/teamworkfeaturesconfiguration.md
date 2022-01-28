---
title: teamworkFeaturesConfiguration 资源类型
description: 表示Microsoft Teams设备Teams客户端配置详细信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cbd95b2fa6a5c20126712abb63eaf00f8c065823
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262467"
---
# <a name="teamworkfeaturesconfiguration-resource-type"></a>teamworkFeaturesConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Microsoft Teams设备Teams客户端配置[详细信息](../resources/teamworkdevice.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|emailToSendLogsAndFeedback|String|用于发送日志和反馈的电子邮件地址。|
|isAutoScreenShareEnabled|Boolean|`True` 如果启用自动屏幕共享。|
|isBluetoothBeaconingEnabled|Boolean|`True`如果蓝牙信号。|
|isHideMeetingNamesEnabled|Boolean|`True` 如果启用隐藏会议名称。|
|isSendLogsAndFeedbackEnabled|Boolean|`True` 如果启用发送日志和反馈。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkFeaturesConfiguration",
  "emailToSendLogsAndFeedback": "String",
  "isAutoScreenShareEnabled": "Boolean",
  "isBluetoothBeaconingEnabled": "Boolean",
  "isHideMeetingNamesEnabled": "Boolean",
  "isSendLogsAndFeedbackEnabled": "Boolean"
}
```

