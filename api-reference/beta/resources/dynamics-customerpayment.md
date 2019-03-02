---
title: customerPayments 资源类型
description: Dynamics 365 Business Central 中的客户付款对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 9063a9066c51956596e4f0aa918a2e7a53bf2ab9
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365610"
---
# <a name="customerpayments-resource-type"></a>customerPayments 资源类型
代表 Dynamics 365 Business Central 中的客户付款。 客户付款作为客户付款日志中的一条线路输入。

## <a name="methods"></a>方法

| 方法         | 返回类型  |说明|
|:---------------|:-------------|:----------|
|[获取 customerPayments](../api/dynamics-customerpayment-get.md)|customerPayments|获取客户付款。|
|[Post customerPayments](../api/dynamics-create-customerpayment.md)|customerPayments|创建客户付款。|
|[修补程序 customerPayments](../api/dynamics-customerpayment-update.md)|customerPayments|更新客户付款。|
|[删除 customerPayments](../api/dynamics-customerpayment-delete.md)|无|删除客户付款。|

## <a name="properties"></a>属性
| 属性     | 类型    |说明|
|:-------------|:--------|:----------|
|id|GUID|客户付款的唯一 ID。 不可编辑。|
|journalDisplayName|string|付款记录所在的行的客户付款日志。|
|lineNumber|integer|客户付款的编号。|
|customerId|GUID|与付款相关的客户的唯一 ID。|
|customerNumber|字符串, 最大大小为20|与付款相关的客户的编号。|
|contactId|字符串, 最大大小为250|给定客户的 exchange 联系人 id。 如果未指定客户 id, 我们将使用联系人 id 来查找它。|
|postingDate|date|客户付款的过帐日期。|
|documentNumber|字符串, 最大大小为20|指定客户付款的文档编号。|
|externalDocumentNumber|字符串, 最大大小为20|指定客户付款的外部文档编号。|
|量|decimal|指定客户付款包含的总金额 (包括 VAT)。|
|appliesToInvoiceId|GUID|与付款相关的发票的唯一 ID。|
|appliesToInvoiceNumber|字符串, 最大大小为20|与付款相关的发票的编号。|
|说明|字符串, 最大大小为50|客户付款的说明, 由用户或 autocreated 提供。|
|批注|字符串, 最大大小为250|用户在客户付款上指定的注释。|
|lastModifiedDateTime|datetime|客户付款修改后的最后一个日期/时间。 只读。|


## <a name="relationships"></a>关系
客户付款是客户付款日志的子页面。 不能直接访问它。

客户付款可以是维行的 "父实体"。

客户 (customerId) 必须存在于 Customers 表中。

发票 (appliesToInvoiceId) 必须存在于 "销售发票" 表中。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "customerId": "GUID",
    "customerNumber": "string",
    "contactId": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "appliesToInvoiceId": "GUID",
    "appliesToInvoiceNumber": "string",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```

