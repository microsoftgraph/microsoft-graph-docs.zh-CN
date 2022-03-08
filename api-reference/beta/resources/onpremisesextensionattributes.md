---
title: onPremisesExtensionAttributes 资源类型
description: user **实体的 onPremisesExtensionAttributes** 属性包含十五个自定义扩展属性。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: a6449c2dd5a437244a5da47e2cf32fefc5e68382
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63331870"
---
# <a name="onpremisesextensionattributes-resource-type"></a>onPremisesExtensionAttributes 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户对象的 **onPremisesExtensionAttributes** 属性和设备对象的 **extensionAttributes** 属性的 [返回](device.md)类型。[](user.md) 返回 15 个自定义扩展属性。

在 [用户](user.md)实体和 **onPremisesSyncEnabled** 用户中，这组属性的颁发机构源是同步到 Azure AD 且只读本地 Active Directory。 对于仅云用户 (**onPremisesSyncEnabled** `false` `null` 为 或) ，可以在创建或更新期间设置 [这些属性](../api/user-update.md)。[](../api/user-post-users.md) 如果以前从本地 Active Directory 同步了仅云用户，则这些属性无法通过 Microsoft Graph API 进行管理。 相反，可以通过 PowerShell 中的 Exchange 管理中心或 Exchange Online V2 模块进行管理。

**设备实体的 extensionAttributes** 属性 [](device.md)仅在设备创建Azure AD更新 [期间](../api/device-post-devices.md)在设备上 [进行管理](../api/device-update.md)。

> **注意：** 这些扩展属性也称为自定义Exchange 1-15。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|extensionAttribute1|String| 第一个可自定义的扩展属性。 |
|extensionAttribute2|String| 第二个可自定义的扩展属性。 |
|extensionAttribute3|字符串| 第三个可自定义的扩展属性。 |
|extensionAttribute4|String| 第四个可自定义的扩展属性。 |
|extensionAttribute5|字符串| 第五个可自定义的扩展属性。 |
|extensionAttribute6|字符串| 第六个可自定义的扩展属性。 |
|extensionAttribute7|String| 第七个可自定义的扩展属性。 |
|extensionAttribute8|String| 第八个可自定义的扩展属性。 |
|extensionAttribute9|String| 第九个可自定义的扩展属性。 |
|extensionAttribute10|字符串| 第十个可自定义的扩展属性。 |
|extensionAttribute11|String| 第十一个可自定义的扩展属性。 |
|extensionAttribute12|String| 第十二个可自定义的扩展属性。 |
|extensionAttribute13|String| 第十三个可自定义的扩展属性。 |
|extensionAttribute14|字符串| 第十四个可自定义的扩展属性。 |
|extensionAttribute15|String| 第十五个可自定义的扩展属性。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


