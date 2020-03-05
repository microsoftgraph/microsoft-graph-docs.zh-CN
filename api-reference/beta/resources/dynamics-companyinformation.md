---
title: companyInformation 资源类型
description: Dynamics 365 Business Central 中的公司信息。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ce982e7d03e4b2e5947381173d57706f6cf8f41e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505124"
---
# <a name="companyinformation-resource-type"></a>companyInformation 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示为 Dynamics 365 Business Central 中的当前公司指定的信息，例如名称、地址、电子邮件地址和网站地址。

## <a name="methods"></a>方法

| 方法         | 返回类型  |说明|
|:---------------|:-------------|:----------|
|[获取 companyInformation](../api/dynamics-companyinformation-get.md)|companyInformation|获取公司信息。|
|[修补程序 companyInformation](../api/dynamics-companyinformation-update.md)|companyInformation|更新公司信息。|


## <a name="properties"></a>属性
| 属性     | 类型      |说明                           |
|:-------------|:--------|:-------------------------------------|
|id            |GUID|公司的唯一 ID。 不可编辑。|
|displayName   |string   |公司的显示名称。           |
|address       |[翻.省略](../resources/dynamics-complextypes.md)|公司地址。 查看复杂类型以获取其他详细信息。|
|phoneNumber   |string   |公司的电话号码。       |
|faxNumber     |string   |公司的传真号码。             |
|email         |string   |公司的电子邮件地址。          |
|website       |string   |公司的网站地址。        |
|taxRegistrationNumber|string|公司的税务登记编号。|
|currencyCode  |string   |公司参与业务的货币。 只读。|
|currentFiscalYearStartDate|date|公司的当前会计年度开始日期。 只读。|
|领域      |string   |公司所属的行业。  |
|头像       |stream   |公司徽标。 只读。          |
|businessProfileId|string|链接到财务公司的业务配置文件 ID。 只读。|
|lastModifiedDateTime|datetime|上次修改公司的日期/时间。 只读。|  


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是 companyInformation 的 JSON 表示形式
```json
{
  "id": "GUID",
  "displayName": "string",
  "address": "NAV.PostalAddress",
  "phoneNumber": "string",
  "faxNumber": "string",
  "email": "string",
  "website": "string",
  "taxRegistrationNumber": "string",
  "currencyCode": "string",
  "currentFiscalYearStartDate": "date",
  "industry": "string",
  "picture": "stream",
  "businessProfileId": "string",
  "lastModifiedDateTime": "datetime"
}

```

