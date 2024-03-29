---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。directoryObject 类型是许多其他目录实体类型（通常称为目录对象）的基类型。
ms.localizationpriority: high
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 95d926deef7961bedd1ebcf9e2ad38f1b7513415
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441417"
---
# <a name="directoryobject-resource-type"></a>directoryObject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 对象。 **directoryObject** 类型是以下目录实体类型（通常称为目录对象）的基类型：

+ [application](application.md)
+ [administrativeUnit](administrativeunit.md)
+ [appRoleAssignment](approleassignment.md)
+ [directoryObject](directoryobject.md)
+ [directoryRole](directoryrole.md)
+ [设备](device.md)
+ [组](group.md)
+ [orgContact](orgcontact.md)
+ [oauth2PermissionGrant](oauth2permissiongrant.md)
+ [servicePrincipal](serviceprincipal.md)
+ [用户](user.md)

该资源支持：

- 通过提供 **delta** 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |读取 directory 对象的属性。|
|[删除](../api/directoryobject-delete.md) | 无 |删除 directory 对象。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|字符串集合|检查指定组列表中的成员身份，并从该列表返回指定用户、组、服务主体、组织联系人或目录对象所属的组。检查是可传递的。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String 集合|返回用户、组、服务主体、组织联系人、设备或目录对象所属的所有组。检查是可传递的。|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|String 集合|检查指定用户、组、设备、组织联系人或目录对象的组、管理单元或目录角色列表中的成员身份。此方法是可传递的。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String 集合| 返回用户、组、设备、组织联系人或目录对象所属的所有组、管理单元和目录角色。检查是可传递的。 |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md) 集合 | 基于提供的 ID 集获取目录对象集。 |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| 验证 Microsoft 365 组的显示名称或邮件昵称是否符合命名策略。 |
|delta|[directoryObject](directoryObject.md) 集合| 获取目录对象的增量更改，例如，[用户](../api/user-delta.md)、[组](../api/group-delta.md)、[应用程序](../api/application-delta.md)和[服务主体](../api/serviceprincipal-delta.md)。 每个派生类型都支持按 **id** 进行筛选。有关 delta 查询的详细信息，请参阅 [使用 delta 查询跟踪 Microsoft Graph 数据中的更改](/graph/delta-query-overview)。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|deletedDateTime|DateTimeOffset|删除此对象的日期和时间。 在对象尚未删除时始终为 `null`。 |
|id|String|对象的唯一标识符。例如，12345678-9 abc-def0-1234-56789 abcde。**id** 属性的值通常（但不总是）用 GUID 表示；将它视为不透明标识符，不要总将它视为 GUID。不可为 null。只读。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


