---
title: authenticationDetail 资源类型
description: 提供用户登录的身份验证详细信息，如多因素身份验证（MFA）信息和 PTA/PHS 详细信息。
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cdfd2abff4d947f7b51a6be0fa8bb81c1413f9c1
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845288"
---
# <a name="authenticationdetail-resource-type"></a>authenticationDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

提供用户登录的身份验证详细信息，如多因素身份验证（MFA）信息和 PTA/PHS 详细信息。

## <a name="properties"></a>属性

| 属性                       | 类型           | Description                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| authenticationMethod           | String         | 用于执行此身份验证步骤的身份验证方法的类型。 可能的值： `Password` 、、、、 `SMS` `Voice` `Authenticator App` `Software OATH token` 、 `Satisfied by token` 。                            |
| authenticationMethodDetail     | String         | 有关用于执行此身份验证步骤的身份验证方法的详细信息。 例如，电话号码（用于短信和语音）、设备名称（用于验证器应用）和密码源（例如，云、AD FS、PTA、PHS）。 |
| authenticationStepDateTime     | DateTimeOffset | 表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。                                           |
| authenticationStepRequirement  | String         | 满足此要求的身份验证步骤。 例如，主身份验证或多重身份验证。                                                                                                     |
| authenticationStepResultDetail | String         | 有关步骤成功或失败的原因的详细信息。 例如，阻止用户、输入欺诈代码、无电话输入超时、无法连接电话或令牌中的声明。                                                     |
| 完成                      | Boolean        | 指示身份验证步骤的状态。 可能的值： `succeeded` 、 `failed` 。                                                                                                                                 |

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