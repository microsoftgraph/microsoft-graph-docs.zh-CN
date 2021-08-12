---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 13a8f055d61037e3d346add591adfd90c6d7a5a98942e6dbd96a021ed1c2bdef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177994"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>resourceSpecificPermissionGrant 资源类型

命名空间：microsoft.graph

resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。

有关授予应用同意访问资源的特定实例的权限，请参阅特定于 [资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。

## <a name="methods"></a>方法

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