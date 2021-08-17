---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 221576c08af5e97979d2a42e8dc0cce483e3bf35
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264155"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>resourceSpecificPermissionGrant 资源类型

命名空间：microsoft.graph

声明已授予特定 Azure AD 应用的权限，用于 Microsoft Graph。

有关授予应用同意访问资源的特定实例的权限，请参阅特定于 [资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

## <a name="methods"></a>Methods

|  方法                                                                   |  返回类型                                                                     | 说明                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[列出组的权限管理](../api/group-list-permissiongrants.md) | [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合 | 列出特定组中已授予的资源特定 [权限](group.md)。 |

## <a name="properties"></a>属性

| 属性        | 类型          | 说明                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | string        | 特定于资源的权限授予的唯一标识符。 只读。           |
| deletedDateTime | dateTimeOffset| 未使用。                                                                             |
| clientId        | string        | 已授予访问权限的 Azure AD 应用的 ID。 只读。                            |
| clientAppId     | string        | 已授予访问权限的 Azure AD 应用的服务主体的 ID。 只读。   |
| resourceAppId   | string        | 托管资源的 Azure AD 应用的 ID。 只读。                        |
| permissionType  | string        | 权限的类型。 可能的值是：`Application`、`Delegated`。 只读。 |
| permission      | string        | 特定于资源的权限的名称。 只读。                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
}-->

```json
{
  "id": "string (identifier)",
  "deletedDateTime": "dateTimeOffset",
  "clientId": "string",
  "clientAppId": "string",
  "resourceAppId": "string",
  "permissionType": "string",
  "permission": "string"
}
```
