---
title: iosNotificationSettings 资源类型
description: 说明通知设置的项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2876146e7e20ad94a7356f623a5b2e17443a18f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172700"
---
# <a name="iosnotificationsettings-resource-type"></a>iosNotificationSettings 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

说明通知设置的项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleID|String|要向其应用这些通知设置的应用的捆绑 ID。|
|appName|String|要与 bundleID 关联的应用程序名称。|
|发布者|String|要与 bundleID 关联的发布者。|
|enabled|Boolean|指示是否允许此应用使用通知。|
|showInNotificationCenter|Boolean|指示是否可以在通知中心中显示通知。|
|showOnLockScreen|Boolean|指示是否可以在锁定屏幕上显示通知。|
|alertType|[iosNotificationAlertType](../resources/intune-deviceconfig-iosnotificationalerttype.md)|指示此应用的通知的警报类型。 可取值为：`deviceDefault`、`banner`、`modal`、`none`。|
|badgesEnabled|Boolean|指示是否允许此应用使用徽章。|
|soundsEnabled|布尔值|指示是否允许此应用使用声音。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```




