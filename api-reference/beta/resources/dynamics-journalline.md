---
title: journalLines 资源类型
description: Dynamics 365 Business Central 中的日志行。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: cb9b20d7d88159dbddd2a18caa6db7fe52e5a601
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972913"
---
# <a name="journallines-resource-type"></a>journalLines 资源类型
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
|journalDisplayName    |字符串, 最大值为10 |此行所属的日记的显示名称。 只读。|
|lineNumber            |integer                 |日志行的编号。                                    |
|accountId             |GUID                    |与日志行相关的帐户的唯一 ID。  |
|accountNumber         |字符串, 最大大小为20 |与日志行相关的帐户的编号。     |
|postingDate           |date                    |日志行的过帐日期。                          |
|documentNumber        |字符串, 最大大小为20 |指定日记行的文档编号。                  |
|externalDocumentNumber|字符串, 最大大小为20 |指定日记行的外部文档编号。        |
|量                |数位                 |指定日记行所包含的总金额 (包括 VAT)。|
|说明           |字符串, 最大大小为50 |日记行的说明, 由用户或 autocreated 提供。|
|注释               |字符串, 最大大小为250|用户在日志行上指定的注释。                      |
|lastModifiedDateTime  |datetime                |修改日记行的最后一个日期/时间。 只读。        |

## <a name="relationships"></a>关系
日志行是日记的子页。 不能直接访问它。

日志行可以是维行的 "父实体"。

帐户 (accountId) 必须存在于 "帐户" 表中。


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
