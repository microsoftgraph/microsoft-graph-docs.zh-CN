---
title: 帐户资源类型
description: Dynamics 365 Business Central 中的 account 对象。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4252c20e9d11f67a6de40871b1649a165cbd787c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507572"
---
# <a name="accounts-resource-type"></a>帐户资源类型
表示 Dynamics 365 Business Central 中的 account 对象。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取帐户](../api/dynamics-account-get.md)|accounts|获取帐户对象。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|GUID|帐户的唯一 ID。|
|number|字符串, 最大大小为20|指定 G/L 帐号的号码。|
|displayName|字符串, 最大大小为50|指定 G/L 帐户的名称。|
|category|字符串, 最大大小为20|指定 G/L 帐户的类别。|
|子类别|字符串, 最大大小为80|指定 G/L 帐户的帐户类别的子类别。|
|堵塞|布尔|指定无法将条目投递到 G/L 帐户。 **如果为 True** , 则表示帐户被阻止, 不允许进行发布。|
|lastModifiedDateTime|datetime|帐户修改后的最后一个日期/时间。|


## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
  "id": "GUID",
  "number": "string",
  "displayName": "string",
  "category": "string",
  "subCategory": "string",
  "blocked": "boolean",
  "lastModifiedDateTime": "datetime"
}

```
