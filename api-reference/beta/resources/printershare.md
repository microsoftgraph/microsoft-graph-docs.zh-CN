---
title: printerShare 资源类型
description: 表示可供用户和打印应用程序发现的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5acbcdc58b730404a39af1f3069b3433fac54ed3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217345"
---
# <a name="printershare-resource-type"></a>printerShare 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可供用户和打印应用程序发现的打印机。

## <a name="methods"></a>Methods

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [List](../api/print-list-shares.md) | [printerShare](printershare.md)集合 | 获取租户中的打印机共享的列表。 |
| [获取](../api/printershare-get.md) | [printerShare](printershare.md) | 读取**printerShare**对象的属性和关系。 |
| [更新](../api/printershare-update.md) | [printerShare](printershare.md) | 更新**printerShare**对象。 |
| [删除](../api/printershare-delete.md) | 无 | 取消打印机的共享。 |
| [列出 allowedUsers](../api/printershare-list-allowedusers.md) | [printUserIdentity](printuseridentity.md)集合 | 检索已授予访问权限以将打印作业提交到关联的打印机共享的用户列表。 |
| [添加 allowedUser](../api/printershare-post-allowedusers.md) | 无 | 向指定的用户授予将打印作业提交到关联的打印机共享的权限。 |
| [删除 allowedUser](../api/printershare-delete-alloweduser.md) | 无 | 撤销指定用户的打印机共享访问权限。 |
| [列出 allowedGroups](../api/printershare-list-allowedgroups.md) | [printIdentity](printidentity.md)集合 | 检索已授予访问权限的组列表，以将打印作业提交到关联的打印机共享。 |
| [添加 allowedGroup](../api/printershare-post-allowedgroups.md) | 无 | 向指定的组授予将打印作业提交到关联的打印机共享的权限。 |
| [删除 allowedGroup](../api/printershare-delete-allowedgroup.md) | 无 | 撤销指定组的打印机共享访问权限。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| PrinterShare 的标识符。 只读。|
|displayName|字符串|打印客户端应显示的打印机共享的名称。|
|createdDateTime|DateTimeOffset|创建打印机共享时的 DateTimeOffset。 只读。|
|manufacturer|String|与此打印机共享关联的打印机报告的制造商。 只读。|
|model|String|与此打印机共享关联的打印机报告的模型名称。 只读。|
|isAcceptingJobs|Boolean|与此打印机共享关联的打印机当前是否正在接受新的打印作业。|
|缺省值|[printerDefaults](printerdefaults.md)|与此打印机共享关联的打印机的默认打印设置。|
|capabilities|[printerCapabilities](printercapabilities.md)|与此打印机共享相关联的打印机的功能。|
|位置|[printerLocation](printerlocation.md)|与此打印机共享关联的打印机的物理和/或组织位置。|
|status|[printerStatus](printerstatus.md)|与此打印机共享关联的打印机的处理状态，包括任何错误。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|印刷|[印刷](printer.md)|与此打印机共享相关联的打印机。 |
|allowedUsers|[printUserIdentity](printuseridentity.md)集合|有权使用打印机打印的用户。|
|allowedGroups|[printIdentity](printidentity.md)|其用户有权使用打印机打印的组。|
|jobs|[printJob](printjob.md)集合| 与此打印机共享关联的打印机排队等待打印的作业列表。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerShare",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerShare resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
