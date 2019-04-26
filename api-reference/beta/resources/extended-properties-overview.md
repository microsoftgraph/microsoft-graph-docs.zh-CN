---
title: Outlook 扩展属性概述
description: '扩展属性允许存储自定义数据, 并专门用作应用程序访问的回退机制 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 38aefd484d4afe13418255aa1d6e0b46050ae4fe
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340301"
---
# <a name="outlook-extended-properties-overview"></a>Outlook 扩展属性概述

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

可以使用以下三种格式之一指定扩展属性的**id** :

- 作为命名属性, 由扩展属性类型、命名空间和字符串名称标识。
- 作为命名属性, 由扩展属性类型、命名空间和数字标识符标识。
- 在属性标记格式中, 由扩展属性类型和[MAPI 属性标记](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-tags)标识。

接下来的2个表描述了应用于单值和多值扩展属性的这些格式。 {_type_} 表示值的类型或扩展属性的值。 示例中使用的是 string、integer 和这些类型的数组。

**单值扩展属性的有效 id 格式**

|**格式**|**示例**|**描述**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"String {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 通过该属性所属的命名空间 (GUID) 和一个字符串名称来标识该属性。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"Integer {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8012"```        | 通过它所属的命名空间 (GUID) 和数字标识符标识属性。  |
| "{_type_} {_属性标记_}"                    | ```"String 0x4001001E"```                                           | 按属性标记标识预定义属性。 |

**多值扩展属性的有效 id 格式**

|**格式**|**示例**|**描述**|
|:---------|:----------|:--------------|
| "{_type_} {_guid_} **Name** {_name_}" | ```"StringArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Name TestProperty"``` | 通过命名空间 (GUID) 和字符串名称标识属性。         |
| "{_type_} {_guid_} **Id** {_id_}"     | ```"IntegerArray {8ECCC264-6880-4EBE-992F-8888D2EEAA1D} Id 0x8013"```        | 通过命名空间 (GUID) 和数字标识符标识属性。   |
| "{_type_} {_属性标记_}"                    | ```"StringArray 0x4002101E"```                                           | 按属性标记标识预定义属性。 |


使用任一命名属性格式将单个值或多值扩展属性定义为自定义属性。 在这两种格式中, 第一个采用字符串名称 (**名称**) 的格式是易于参考的首选格式。 命名属性在 0x8000-0xfffe 范围中具有其[属性标识符](https://docs.microsoft.com/en-us/office/client-developer/outlook/mapi/mapi-property-identifier-overview)。

使用属性标记格式访问由 MAPI、客户端或服务器预定义且尚未在 Microsoft Graph 中公开的属性。 这些属性在 0x0001-0x7fff 范围中具有属性标识符。 请勿尝试使用属性标记格式定义自定义属性。 

在 \[MS-OXPROPS\] Microsoft Corporation 的[“Exchange Server 协议 Master 属性列表”](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx)中，可以了解如何将扩展属性映射到现有 MAPI 属性，如属性标识符和 GUID。

**注意**：为 **id** 选择一种格式后，只能按此格式访问扩展属性。

## <a name="rest-api-operations"></a>REST API 操作
 
单值扩展属性的操作：

- [在新建或现有的资源实例中创建扩展属性](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md)
- [使用 `$expand` 或 `$filter` 获取一个包含扩展属性的资源实例或资源实例集合](../api/singlevaluelegacyextendedproperty-get.md)

多值扩展属性的操作：

- [在新建或现有的资源实例中创建扩展属性](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md)
- [使用 `$expand` 获取一个包含扩展属性的资源实例](../api/multivaluelegacyextendedproperty-get.md)

