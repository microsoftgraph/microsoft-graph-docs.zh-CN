---
title: 供应商资源类型
description: Dynamics 365 Business Central 中的供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: a2102a77748ebef8267792a887a522fa716619ab
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040038"
---
# <a name="vendors-resource-type"></a>供应商资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的供应商。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取供应商](../api/dynamics-vendor-get.md)|供应商|获取一个供应商对象。|
|[供应商后](../api/dynamics-create-vendor.md)|供应商|创建一个供应商对象。|
|[修补程序供应商](../api/dynamics-vendor-update.md)|供应商|更新供应商对象。|
|[删除供应商](../api/dynamics-vendor-delete.md)|无|删除 "供应商" 对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|供应商的唯一 ID。 不可编辑。|
|数字|string|供应商编号。|
|displayName|string|供应商的显示名称。|
|address|[翻.省略](../resources/dynamics-complextypes.md)|供应商的地址。|
|phoneNumber|string|供应商的电话号码。|
|email|string|供应商的电子邮件地址。|
|website|string|供应商的网站地址。|
|taxRegistrationNumber|string|供应商的税务登记编号。|
|currencyId|GUID|供应商的默认币种代码 ID。|
|currencyCode|string|供应商的默认币种代码。|
|irs1099Code|string|指定供应商的1099代码。 仅限美国。|
|paymentTermsId|GUID|供应商的默认付款条款 ID。|
|paymentMethodId|GUID|供应商的默认付款方法 ID。|
|taxLiable|boolean|指定供应商是否对税负有责任。|
|堵塞|string|指定哪些交易记录与供应商不能过帐。 接受的值为空、付款或全部|
|恰好|数位|供应商的余额。 只读。|
|lastModifiedDateTime|datetime|上次修改供应商的日期/时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是供应商的 JSON 表示形式。

```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyId": "GUID",
  "currencyCode": "string",
  "irs1099Code": "string",
  "paymentTermsId": "GUID",
  "paymentMethodId": "GUID",
  "taxLiable": "boolean",
  "blocked": "string",
  "balance": "decimal",
  "lastModifiedDateTime": "datetime"
}

```



