---
title: 服务根
description: 2015-10-25 14:57:30 UTC->
localization_priority: Normal
ms.openlocfilehash: 5e9c464c50dcbef7a03ca3a2fc2b0aaac40fbb30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524308"
---
# <a name="service-root"></a>服务根

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>方法



| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建设备](../api/device-post-devices.md) |[设备](device.md)| 通过发布到设备集合创建新设备。|
|[列出设备](../api/device-list.md) | [设备](device.md)集合 |获取 device 对象集合。 |
|[激活 directoryRole](../api/directoryrole-post-directoryroles.md) | [directoryRole](directoryrole.md) |激活目录角色。 |
|[列出 directoryRole](../api/directoryrole-list.md) | [directoryRole](directoryrole.md) 集合 |获取 directoryRole 对象集合。 |
|[列出 directoryRoleTemplate](../api/directoryroletemplate-list.md) | [directoryRoleTemplate](directoryroletemplate.md) 集合 |获取 directoryRoleTemplate 对象集合。 |
|[列出驱动器](../api/drive-list.md) | [驱动器](drive.md) 集合 |获取 drive 对象集合。 |
|[获取驱动器](../api/drive-get.md) | [驱动器](drive.md)  |获取 drive 对象的属性。 |
|[创建组](../api/group-post-groups.md) |[组](group.md)| 通过发布到组集合创建新组。|
|[列出组](../api/group-list.md) | [组](group.md) 集合 |获取 group 对象集合。 |
|[列出组织](../api/organization-list.md) | [组织](organization.md) 集合 |获取 organization 对象集合。 |
|[列出 subscribedSku](../api/subscribedsku-list.md) | [subscribedSku](subscribedsku.md) 集合 |获取 subscribedSku 对象集合。 |
|[创建用户](../api/user-post-users.md) |[用户](user.md)| 通过发布到用户集合创建新用户。|
|[列出用户](../api/user-list.md) | [用户](user.md) 集合 |获取 user 对象集合。 |
|[创建 connectorGroup](../api/connectorgroup-post-connectorgroups.md) |[connectorGroup](connectorgroup.md)|通过发布到 connectorGroups 集合中创建新 connectorGroup。|
|[列表 connectorGroup](../api/connectorgroup-list.md) | [connectorGroup](connectorgroup.md)集合 |获取 connectorGroup 对象集合。 |
|[列表连接器](../api/connector-list.md) | [连接器](connector.md)集合 |获取连接器对象集合。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/service-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
