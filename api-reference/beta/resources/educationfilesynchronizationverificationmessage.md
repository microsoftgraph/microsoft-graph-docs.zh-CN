---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 表示返回给客户端以响应对基于 CSV 的学校数据配置文件的启动同步的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据，然后再重新启动请求，才能与 Azure Active Directory （Azure AD）同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 45f439adaf45ade7e63dd4cde8ed72852244192c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502002"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示返回给客户端以响应对基于 CSV 的学校数据配置文件的[启动同步](../api/educationsynchronizationprofile-start.md)的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据，然后再重新启动请求，才能与 Azure Active Directory （Azure AD）同步。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:-|:-|:-|
| **类型** | string | 邮件的类型。 可取值为：`error`、`warning`、`information`。 | 
| **filename** | string | 包含错误的源文件。 |
| **说明** | string | 有关邮件类型的详细信息。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
