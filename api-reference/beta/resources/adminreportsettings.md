---
title: adminReportSettings 资源类型
description: 表示 Microsoft 365 报表的租户级设置。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: reports
author: qiwhuang
ms.openlocfilehash: faa1073175ca09ef4aee52ecfe55d92d24409687
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856530"
---
# <a name="adminreportsettings-resource-type"></a>adminReportSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 365 报表的租户级设置。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[获取 adminReportSettings](../api/adminreportsettings-get.md)|[adminReportSettings](../resources/adminreportsettings.md)|获取 Microsoft 365 报表的租户级设置。|
|[更新 adminReportSettings](../api/adminreportsettings-update.md)|[adminReportSettings](../resources/adminreportsettings.md)|更新 Microsoft 365 报表的租户级别设置。|

## <a name="properties"></a>属性

| 属性       | 类型           | Description                                 |
| -------------- | -------------- | ------------------------------------------- |
| displayConcealedNames | Boolean | 如果设置为 `true`，所有报表都将隐藏用户名、组和网站等用户信息。 如果 `false`，所有报表都将显示可识别的信息。 此属性表示Microsoft 365 管理中心中的设置。 此为必需属性。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminReportSettings",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminReportSettings",
  "displayConcealedNames": "Boolean"
}
```
