---
title: Outlook 扩展属性概述
description: '扩展的属性允许存储自定义数据和专门用作应用程序访问的回退机制 '
ms.openlocfilehash: a15c44c832971d0fc91cd1cc9e9c29db80715130
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046465"
---
# <a name="outlook-extended-properties-overview"></a>Outlook 扩展属性概述

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

扩展属性允许存储自定义数据，当 Outlook MAPI 属性_尚未在 Microsoft Graph API 元数据中公开_时，扩展属性专门用作应用访问这些属性的自定义数据的回退机制。可以使用扩展属性 REST API 在以下用户资源中存储或获取此类自定义数据：

- [邮件](../resources/message.md)
- [mailFolder](../resources/mailfolder.md)
- [事件](../resources/event.md)
- [日历](../resources/calendar.md)
- [联系人](../resources/contact.md)
- [contactFolder](../resources/contactfolder.md)
- [Outlook 任务](../resources/outlooktask.md)
- [Outlook 任务文件夹](../resources/outlooktaskfolder.md) 

或者，在以下 Office 365 组资源中：

- 组 [事件](../resources/event.md)
- 组 [日历](../resources/calendar.md)
- 组[帖子](../resources/post.md) 

## <a name="use-extended-properties-or-open-extensions"></a>使用扩展属性还是开放扩展？

在大多数的常见情况下，你应该能够使用开放扩展（用 [openTypeExtension](../resources/opentypeextension.md) 表示，以前被称为 Office 365 数据扩展）来存储和访问用户邮箱中资源实例的自定义数据。仅当需要访问尚未通过 [Microsoft Graph API 元数据](https://developer.microsoft.com/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据时使用扩展属性。

## <a name="types-of-extended-properties"></a>扩展属性的类型

根据是否打算将单个值或多个值（相同类型）存储在一个扩展属性中，可以将扩展属性创建为 [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) 或 [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)。

其中的每种类型都通过其 **id** 进行标识并将数据存储在 **value** 中。 

可以使用 **id** 获取特定的资源实例以及该扩展属性，或筛选单值扩展属性以获取拥有该属性的所有实例。 

**注意** 不能使用 REST API 在一个调用中获取特定实例的所有扩展属性。
  

### <a name="id-formats"></a>id 格式

您可以在三种格式之一指定的扩展属性的**id** :

- 为扩展的属性类型、 命名空间和字符串名称由标识的命名属性。
- 为扩展的属性类型、 命名空间和一个数字标识符标识的命名属性。
- 在由扩展的属性类型和[MAPI 属性标记](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)标识属性标记格式。

接下来的两个表介绍这些格式为单角色和多值应用于的扩展属性。 {_类型_} 表示的扩展属性的值的类型。 示例中使用的是 string、integer 和这些类型的数组。

**单值扩展属性的有效 id 格式**

|**格式**|**示例**|**说明**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 标识属性由其所属的命名空间 (GUID) 和字符串名称。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | 标识通过其所属的命名空间 (GUID) 和一个数字标识符的属性。  |
| "{_类型_} {_属性标记_}"                    | ```"String 0x4001001E"```                                           | 根据属性标记标识的预定义的属性。 |

**多值扩展属性的有效 id 格式**

|**格式**|**示例**|**说明**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 标识属性的命名空间 (GUID) 和字符串名称。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | 标识属性的命名空间 (GUID) 和数字的标识符。   |
| "{_类型_} {_属性标记_}"                    | ```"StringArray 0x4002101E"```                                           | 根据属性标记标识的预定义的属性。 |


使用的命名的属性的格式之一以定义一个或多值单值的扩展的属性为自定义属性。 之间的两个格式，第一个采用字符串名称 （**Name**） 是为了便于引用的首选的格式。 命名的属性中 0x8000 0xfffe 有及其[属性标识符](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)范围。

使用属性标记格式访问通过 MAPI，或客户端或服务器，预定义的属性和的具有不已经暴露在 Microsoft Graph 中。 这些属性中 0x0001 0x7fff 有属性标识符范围。 不要尝试定义使用属性标记格式的自定义属性。 

在 \[MS-OXPROPS\] Microsoft Corporation 的[“Exchange Server 协议 Master 属性列表”](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)中，可以了解如何将扩展属性映射到现有 MAPI 属性，如属性标识符和 GUID。

**注意**：为 **id** 选择一种格式后，只能按此格式访问扩展属性。

## <a name="rest-api-operations"></a>REST API 操作
 
单值扩展属性的操作：

- [在新建或现有的资源实例中创建扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [使用 `$expand` 或 `$filter` 获取一个包含扩展属性的资源实例或资源实例集合](../api/singlevaluelegacyextendedproperty-get.md)

多值扩展属性的操作：

- [在新建或现有的资源实例中创建扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [使用 `$expand` 获取一个包含扩展属性的资源实例](../api/multivaluelegacyextendedproperty-get.md)

