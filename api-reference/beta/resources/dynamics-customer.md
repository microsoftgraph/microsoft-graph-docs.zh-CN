---
title: customers 资源类型
description: 代表 Dynamics 365 Business Central 中的客户。
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: c6b39829d2b55dc872d281443eaad1b279715b50
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989708"
---
# <a name="customers-resource-type"></a>customers 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Dynamics 365 Business Central 中的客户。

## <a name="methods"></a>方法

| 方法                                              |返回类型| 说明      |
|:----------------------------------------------------|:----------|:-----------------|
|[获取客户](../api/dynamics-customer-get.md)      |各地   |获取客户。   |
|[创建客户](../api/dynamics-create-customer.md)|各地   |创建客户。|
|[更新客户](../api/dynamics-customer-update.md)|各地   |更新客户。|
|[删除客户](../api/dynamics-customer-delete.md)|无        |删除客户。|

## <a name="properties"></a>属性
| 属性    | 类型     |说明|
|:------------|:---------|:----------|
|id           |GUID      |项目的唯一 ID。 不可编辑。|
|数字       |字符串    |客户编号。|
|displayName  |string    |指定客户的名称。 此名称将显示在客户的所有销售文档中。|
|类型         |string    |指定客户类型，可以是 "Company"，也可以是 "Person"。|
|address      |[翻.省略](../resources/dynamics-complextypes.md)|指定客户地址。 此地址将显示在客户的所有销售文档中。|
|phoneNumber  |字符串    |指定客户的电话号码。|
|email        |string    |指定客户的电子邮件地址。|
|website      |字符串    |指定客户的主页地址。|
|taxLiable    |boolean   |指定客户或供应商是否对销售税负有义务。 如果客户有义务责任，则设置为 **true** 。|
|taxAreaId    |GUID      |指定客户所属的税务区域。|
|taxAreaDisplayName|字符串|指定客户所属的税务区域的显示名称。|
|taxRegistrationNumber|字符串，最大大小为20|指定客户的税务登记编号。|
|currencyId   |GUID      |指定客户使用的货币。|
|currencyCode |位数   |客户的默认货币代码。|
|paymentTermsId|GUID     |指定客户使用的付款期限。|
|paymentMethodId|GUID    |指定客户使用的支付方式。|
|shipmentMethodId|GUID   |指定客户使用的装运方法。|
|堵塞      |字符串    |指定无法对客户的交易记录进行过帐。 设置为 **All**，如果客户被阻止，则设置为空（如果未阻止）。|
|恰好      |位数   |指定客户为完成的销售而支付的付款金额。 此值也称为客户余额。 只读。|
|overdueAmount|位数   |指定客户的逾期金额。|
|totalSalesExcludingTax|位数|指定不包括客户税的总销售额。|
|lastModifiedDateTime|datetime|客户修改后的最后一个日期/时间。 只读。|  


## <a name="relationships"></a>关系
币种 (currencyCode) 必须在货币表中存在。

付款期限 (paymentTerms) 必须存在于付款期限表中。

装运方法表中必须存在 (shipmentMethod) 的装运方法。

付款方法表中必须存在 (paymentMethod) 的付款方式。

税务区域表中必须存在 (taxArea) 的税务区域。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "address": NAV.PostalAddress,
    "phoneNumber": "string",
    "email": "string",
    "website": "string",
    "taxLiable": "boolean",
    "taxAreaId": "GUID",
    "taxAreaDisplayName": "string",
    "taxRegistrationNumber": "string",
    "currencyCode": "string",
    "paymentTermsId": "GUID",
    "shipmentMethodId": "GUID",
    "paymentMethodId":  "GUID",
    "blocked": "string",
    "balance": "decimal",
    "overdueAmount": "numeric",
    "totalSalesExcludingTax": "numeric",
    "lastModifiedDateTime": "datetime"
}


```



