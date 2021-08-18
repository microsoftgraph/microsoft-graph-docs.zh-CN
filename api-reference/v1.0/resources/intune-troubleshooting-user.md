---
title: 用户资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3b0e61f8f85b231ab11377a6811c3ee3e3745ff
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266851"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[List users](../api/intune-troubleshooting-user-list.md)|[user](../resources/intune-troubleshooting-user.md) 集合|列出 [user](../resources/intune-troubleshooting-user.md) 对象的属性和关系。|
|[Get user](../api/intune-troubleshooting-user-get.md)|[user](../resources/intune-troubleshooting-user.md)|读取 [user](../resources/intune-troubleshooting-user.md) 对象的属性和关系。|
|[Create user](../api/intune-troubleshooting-user-create.md)|[user](../resources/intune-troubleshooting-user.md)|创建新的 [user](../resources/intune-troubleshooting-user.md) 对象。|
|[Delete user](../api/intune-troubleshooting-user-delete.md)|None|删除 [user](../resources/intune-troubleshooting-user.md)。|
|[Update user](../api/intune-troubleshooting-user-update.md)|[user](../resources/intune-troubleshooting-user.md)|更新 [user](../resources/intune-troubleshooting-user.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户的唯一标识符|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) 集合|此用户的故障排除事件列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




