---
title: authenticationDetail 资源类型
description: 提供用户登录的身份验证详细信息，例如多重身份验证 (MFA) 和 PTA/PHS 详细信息。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b888ec232a95c821ab00f6baa16e787cfbc7dd7f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136624"
---
# <a name="authenticationdetail-resource-type"></a>authenticationDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用户登录的身份验证详细信息，例如多重身份验证 (MFA) 和 PTA/PHS 详细信息。

## <a name="properties"></a>属性

| 属性                       | 类型           | 说明                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | 字符串         | 用于执行此步骤的身份验证方法的类型。 可能的值： `Password` `SMS` ， ， ， `Voice` `Authenticator App` `Software OATH token` 。 `Satisfied by token`                            |
| authenticationMethodDetail     | 字符串         | 有关用于执行此身份验证步骤的身份验证方法的详细信息。 例如，短信和语音 (的电话号码) 设备名称 (for Authenticator 应用) ，密码源 (例如云、AD FS、PTA、PHS) 。 |
| authenticationStepDateTime     | DateTimeOffset | 表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。                                           |
| authenticationStepRequirement  | 字符串         | 满足此要求的身份验证步骤。 例如，主身份验证或多重身份验证。                                                                                                     |
| authenticationStepResultDetail | 字符串         | 有关步骤成功或失败的原因的详细信息。 例如，阻止用户、输入欺诈代码、无电话输入 - 已注销、电话无法访问或令牌中声明。                                                     |
| succeeded                      | Boolean        | 指示身份验证步骤的状态。 可能的值： `succeeded` `failed` .                                                                                                                                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

