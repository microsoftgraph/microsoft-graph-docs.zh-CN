---
title: cloudPcUserSetting 资源类型
description: 表示云电脑用户设置
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 6e98d64650f3a05dd0629bc1a92a388fa637ad64
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335442"
---
# <a name="cloudpcusersetting-resource-type"></a>cloudPcUserSetting 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑用户设置。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 cloudPcUserSettings](../api/virtualendpoint-list-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md) 集合|获取 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 及其属性的列表。|
|[获取 cloudPcUserSetting](../api/cloudpcusersetting-get.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|读取 [cloudPcUserSetting 对象的属性和](../resources/cloudpcusersetting.md) 关系。|
|[创建 cloudPcUserSetting](../api/virtualendpoint-post-usersettings.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|创建新的 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。|
|[更新 cloudPcUserSetting](../api/cloudpcusersetting-update.md)|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|更新 [cloudPcUserSetting 对象](../resources/cloudpcusersetting.md) 的属性。|
|[删除 cloudPcUserSetting](../api/cloudpcusersetting-delete.md)|无|删除 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 对象。|
|[Assign](../api/cloudpcusersetting-assign.md)|无|将 [cloudPcUserSetting](../resources/cloudpcusersetting.md) 分配给用户组。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|云电脑用户设置的唯一标识符。 只读。|
|displayName|String|用户界面中显示的设置名称。 |
|localAdminEnabled|Boolean|指示是否已启用本地管理员选项。 默认值为 `false`。 若要启用本地管理员选项，将设置更改为 `true`。 如果启用了本地管理员选项，最终用户可以是云电脑设备的管理员。 |
|selfServiceEnabled|Boolean|指示是否已启用自助服务选项。 默认值为 `false`。 若要启用自助服务选项，将设置更改为 `true`。如果启用自助服务选项，则允许最终用户执行一些自助服务操作，例如通过最终用户门户升级云电脑。|
|restorePointSetting|[cloudPcRestorePointSetting](../resources/cloudpcrestorepointsetting.md)|定义创建还原点的频率，即，为用户预配的云电脑拍摄) 快照 (默认值为 12 小时) ，以及是否允许用户将自己的云电脑还原到特定时间点的备份。|
|lastModifiedDateTime|DateTimeOffset|上次修改设置的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。 |
|createdDateTime|DateTimeOffset|创建设置的日期和时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) 集合|表示分配了Microsoft 365 cloudPCUserSetting 的Azure AD组和安全组集。 仅在 `$expand` 上返回。 有关示例，请参阅 [获取 cloudPcUserSettingample](../api/cloudpcusersetting-get.md)。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSetting",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSetting",
  "id": "String (identifier)",
  "displayName": "String",
  "selfServiceEnabled": "Boolean",
  "localAdminEnabled": "Boolean",
  "restorePointSetting": {
    "@odata.type": "microsoft.graph.cloudPcRestorePointSetting"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)"
}
```
