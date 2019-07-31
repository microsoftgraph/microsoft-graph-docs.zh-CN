---
title: customerPaymentJournals 资源类型
description: Dynamics 365 Business Central 中的客户付款日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0791fe2b8c36bdff535f7fc56dea54abe1632647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973630"
---
# <a name="customerpaymentsjournals-resource-type"></a>customerPaymentsJournals 资源类型
表示 Dynamics 365 Business Central 中的客户付款日志。

## <a name="methods"></a>方法

| 方法               | 返回类型             |说明                      |
|:---------------------|:------------------------|:--------------------------------|
|[获取 customerPaymentJournals](../api/dynamics-customerpaymentsjournal-get.md)      |customerPaymentJournals|获取客户付款日志。   |
|[Post customerPaymentJournals](../api/dynamics-create-customerpaymentsjournal.md)  |customerPaymentJournals|创建客户付款日志。|
|[修补程序 customerPaymentJournals](../api/dynamics-customerpaymentsjournal-update.md) |customerPaymentJournals|更新客户付款日志。|
|[删除 customerPaymentJournals](../api/dynamics-customerpaymentsjournal-delete.md)|无                     |删除客户付款日志。|

## <a name="properties"></a>属性
| 属性           | 类型                  |说明                                                             |
|:-------------------|:----------------------|:-----------------------------------------------------------------------|
|id                  |GUID                   |客户付款日志的唯一 ID。 不可编辑。           |
|code                |字符串, 最大值为10| 客户付款日志的代码。                             |
|displayName         |字符串, 最大大小为50| 客户付款日志的显示名称。                     |
|lastModifiedDateTime|datetime               |上次修改客户付款日志的日期/时间。 只读。|

## <a name="relationships"></a>关系

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "datetime"
}
```

