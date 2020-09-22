---
title: journalLines 资源类型
description: Dynamics 365 Business Central 中的日志行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 99d06b5a49bd2881ea6f329e8b0d3692a25444b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013795"
---
# <a name="journallines-resource-type"></a>journalLines 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Dynamics 365 Business Central 中的日记中的一条线。

## <a name="methods"></a>方法

| 方法                                                    | 返回类型|说明         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[获取 journalLines](../api/dynamics-journalline-get.md)      |journalLines|获取日志行。   |
|[Post journalLines](../api/dynamics-create-journalline.md)  |journalLines|创建日志行。|
|[修补程序 journalLines](../api/dynamics-journalline-update.md) |journalLines|更新日记行。|
|[删除 journalLines](../api/dynamics-journalline-delete.md)|无        |删除日志行。|

## <a name="properties"></a>属性
| 属性             | 类型                   |说明                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|id                    |GUID                    |日记行的唯一 ID。 不可编辑。                   |
|journalDisplayName    |字符串，最大值为10 |此行所属的日记的显示名称。 只读。|
|lineNumber            |integer                 |日志行的编号。                                    |
|accountId             |GUID                    |与日志行相关的帐户的唯一 ID。  |
|accountNumber         |字符串，最大大小为20 |与日志行相关的帐户的编号。     |
|postingDate           |date                    |日志行的过帐日期。                          |
|documentNumber        |字符串，最大大小为20 |指定日记行的文档编号。                  |
|externalDocumentNumber|字符串，最大大小为20 |指定日记行的外部文档编号。        |
|量                |数位                 |指定日志行所包含的增值税)  (总金额。|
|description           |字符串，最大大小为50 |日记行的说明，由用户或 autocreated 提供。|
|comment               |字符串，最大大小为250|用户在日志行上指定的注释。                      |
|lastModifiedDateTime  |datetime                |修改日记行的最后一个日期/时间。 只读。        |

## <a name="relationships"></a>关系
日志行是日记的子页。 不能直接访问它。

日志行可以是维行的 "父实体"。

帐户表中必须存在 (accountId) 帐户。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```


