---
title: educationFileSynchronizationVerificationMessage 资源类型
description: 表示返回给客户端以响应对基于 CSV 的学校数据配置文件的启动同步的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据, 然后再重新启动请求, 才能与 azure Active Directory (azure AD) 同步。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bbf38f15fbe14112ef254c625a8747e57eb1cae4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340509"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示返回给客户端以响应对基于 CSV 的学校数据配置文件的[启动同步](../api/educationsynchronizationprofile-start.md)的请求的错误。 资源将包含验证导致的错误。 用户必须先修复源数据, 然后再重新启动请求, 才能与 azure Active Directory (azure AD) 同步。

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
