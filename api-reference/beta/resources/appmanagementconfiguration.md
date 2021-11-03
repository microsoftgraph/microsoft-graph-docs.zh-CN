---
title: appManagementConfiguration 资源类型
description: 应用管理配置对象，该对象包含可配置为对应用程序和服务主体启用各种限制的属性。
author: madansr7
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: c87918a001e5ede8a521f7ff666f902ba9d28b54
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695523"
---
# <a name="appmanagementconfiguration-resource-type"></a>appManagementConfiguration 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

应用管理配置对象，该对象包含可配置为对应用程序和服务主体启用各种限制的属性。

## <a name="properties"></a>属性

| 属性            | 类型                                                                  | 说明                                                                                       |
| :------------------ | :-------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------ |
| passwordCredentials | [passwordCredentialConfiguration](passwordCredentialConfiguration.md) 集合 | 要应用于应用程序或服务主体的密码限制设置的集合。 |
| keyCredentials | [keyCredentialConfiguration](keyCredentialConfiguration.md) 集合 | 要应用于应用程序或服务主体的 keyCredential 限制设置的集合。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appManagementConfiguration"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.appManagementConfiguration",
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredentialConfiguration"
    }
   ],
   "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredentialConfiguration"
    }
   ]
}
```
