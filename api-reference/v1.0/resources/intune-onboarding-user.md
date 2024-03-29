---
title: 用户资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30c01a5217890a639137bbd1989f52d5f9090f86
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731202"
---
# <a name="user-resource-type"></a>用户资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List users](../api/intune-onboarding-user-list.md)|[user](../resources/intune-onboarding-user.md) 集合|列出 [user](../resources/intune-onboarding-user.md) 对象的属性和关系。|
|[Get user](../api/intune-onboarding-user-get.md)|[user](../resources/intune-onboarding-user.md)|读取 [user](../resources/intune-onboarding-user.md) 对象的属性和关系。|
|[Create user](../api/intune-onboarding-user-create.md)|[user](../resources/intune-onboarding-user.md)|创建新的 [user](../resources/intune-onboarding-user.md) 对象。|
|[Delete user](../api/intune-onboarding-user-delete.md)|None|删除 [user](../resources/intune-onboarding-user.md)。|
|[Update user](../api/intune-onboarding-user-update.md)|[user](../resources/intune-onboarding-user.md)|更新 [user](../resources/intune-onboarding-user.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|用户的唯一标识符。|
|deviceEnrollmentLimit|Int32|允许用户注册的最大设备数的限制。 允许的值为 5 或 1000。|

## <a name="relationships"></a>关系
无

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
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 1024
}
```





