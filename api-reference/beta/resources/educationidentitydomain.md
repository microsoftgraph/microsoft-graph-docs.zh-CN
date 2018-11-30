---
title: educationIdentityDomain 资源类型
description: '代表教育用户类型和用户的帐户所属的域之间的映射。 域资源是标识创建配置的一部分。 '
ms.openlocfilehash: 8298e1eb38ae70f982719ee3a7d6588cd181bdd8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046681"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

代表教育用户类型和用户的帐户所属的域之间的映射。 域资源是[标识创建配置](educationidentitycreationconfiguration.md)的一部分。 

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **appliesTo** | string |  要分配许可证的用户角色类型。 可取值为：`student`、`teacher`。      |
| **name** | string |  表示的用户帐户的域。         |

## <a name="json-representation"></a>JSON 表示形式
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
