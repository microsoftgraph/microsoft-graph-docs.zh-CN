---
title: delegatedAdminServiceManagementDetail 资源类型
description: 包含由委派管理的客户租户中服务的管理详细信息。
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 53eca1c8d8d60ea78e080caede5ed7096a6ff825
ms.sourcegitcommit: 5a43129dbf705f2d1a6afcff36af9f41ecee026d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2022
ms.locfileid: "64704161"
---
# <a name="delegatedadminservicemanagementdetail-resource-type"></a>delegatedAdminServiceManagementDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含由委派管理的客户租户中服务的管理详细信息。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 delegatedAdminServiceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md)|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|获取 **delegatedAdminServiceManagementDetail** 对象及其属性的列表。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|托管服务的标识符。 只读。|
|serviceName|String|托管服务的名称。 只读。|
|serviceManagementUrl|String|托管服务的管理门户的 URL。 只读。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminServiceManagementDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminServiceManagementDetail",
  "id": "String (identifier)",
  "serviceName": "String",
  "serviceManagementUrl": "String"
}
```
