---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a34faa7a7b709d85cd2bee3208cc22270fecbe74
ms.sourcegitcommit: 8b1a6d7b0516f936ce4626246408f067527f5082
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/06/2021
ms.locfileid: "51594889"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a>resourceSpecificPermissionGrant 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。

## <a name="methods"></a>方法

|  方法                                                                   |  返回类型                                                                     | Description                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[聊天的列表权限授予](../api/chat-list-permissiongrants.md)   | [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合 | 列出特定聊天中已授予的权限。  |
|[列出组的权限授予](../api/group-list-permissiongrants.md) | [resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合 | 列出特定组中已授予的权限。 |

## <a name="properties"></a>属性

| 属性        | 类型          | 说明                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| id              | string        | 特定于资源的权限授予的唯一标识符。 只读。           |
| deletedDateTime | dateTimeOffset| 未使用。                                                                             |
| clientId        | 字符串        | 已授予访问权限的 Azure AD 应用的 ID。 只读。                            |
| clientAppId     | 字符串        | 已授予访问权限的 Azure AD 应用的服务主体的 ID。 只读。   |
| resourceAppId   | 字符串        | 托管资源的 Azure AD 应用的 ID。 只读。                        |
| permissionType  | 字符串        | 权限的类型。 可能的值是 `Application` `Delegated` ：、。 只读。 |
| permission      | 字符串        | 权限的名称。 只读。                                                |

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


