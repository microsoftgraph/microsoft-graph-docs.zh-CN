---
title: 供应商资源类型
description: Dynamics 365 Business Central 中的供应商对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 0848b6fbb67964faa9565f2ed95120f563c71f53
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50293069"
---
# <a name="vendors-resource-type"></a>供应商资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Dynamics 365 Business Central 中的供应商。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取供应商](../api/dynamics-vendor-get.md)|供应商|获取供应商对象。|
|[发布供应商](../api/dynamics-create-vendor.md)|供应商|创建供应商对象。|
|[修补程序供应商](../api/dynamics-vendor-update.md)|供应商|更新供应商对象。|
|[删除供应商](../api/dynamics-vendor-delete.md)|无|删除供应商对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|供应商的唯一 ID。 不可编辑。|
|number|string|供应商编号。|
|displayName|string|供应商的显示名称。|
|address|[导航。PostalAddress](../resources/dynamics-complextypes.md)|供应商地址。|
|phoneNumber|string|供应商的电话号码。|
|email|string|供应商的电子邮件地址。|
|website|string|供应商的网站地址。|
|taxRegistrationNumber|string|供应商的税务注册号码。|
|currencyId|GUID|供应商的默认货币代码 ID。|
|currencyCode|string|供应商的默认货币代码。|
|irs1099Code|string|为供应商指定 1099 代码。 仅美国。|
|paymentTermsId|GUID|供应商的默认付款条款 ID。|
|paymentMethodId|GUID|供应商的默认付款方式 ID。|
|taxLiable|boolean|指定供应商是否负责纳税。|
|blocked|string|指定无法发布与供应商的哪些事务。 接受的值为空、付款或全部|
|平衡|decimal|供应商的余额。 只读。|
|lastModifiedDateTime|datetime|上次修改供应商的日期时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vendor"
}-->

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



