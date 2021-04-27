---
title: relatedContact 资源类型
description: 与教育用户相关的联系人记录为监护人、助手、儿童等提供相关信息。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4859492f016b88a39c375d3556270f5496b8b318
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035951"
---
# <a name="relatedcontact-resource-type"></a>relatedContact 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与教育用户相关的联系人 [记录为](../resources/educationuser.md) 监护人、助手、儿童等提供相关信息。

## <a name="methods"></a>方法

| 方法                                    | 返回类型                   | 说明                                                             |
| :---------------------------------------- | :---------------------------- | :---------------------------------------------------------------------- |
| [更新](../api/relatedcontact-update.md) | **relatedContact** 集合 | 更新[educationUser 的 relatedContacts](educationuser.md)  |

## <a name="properties"></a>属性

| 属性      | 类型                | 说明                                                                                                                                |
| :------------ | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| displayName   | String              | 联系人的姓名。 必需。                                                                                                             |
| accessConsent | 布尔值             | 指示用户是否已同意访问学生数据。                                                                      |
| emailAddress  | String              | 联系人的电子邮件地址。                                                                                                              |
| mobilePhone   | String              | 联系人的移动电话号码。                                                                                                        |
| 关系  | contactRelationship | 与用户的关系。 可取值为：`parent`、`relative`、`aide`、`doctor`、`guardian`、`child`、`other`、`unknownFutureValue`。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": "Boolean"
}
```
