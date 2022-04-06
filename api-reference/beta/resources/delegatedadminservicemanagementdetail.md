---
title: delegatedAdminServiceManagementDetail 资源类型
description: 包含由委派管理的客户租户中服务的管理详细信息。
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 837a7377031b7b2b913cf9346f8ca151da0267e1
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589593"
---
# <a name="delegatedadminservicemanagementdetail-resource-type"></a>delegatedAdminServiceManagementDetail 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含由委派管理的客户租户中服务的管理详细信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 delegatedAdminServiceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md)|[delegatedAdminServiceManagementDetail](delegatedadminservicemanagementdetail.md)|获取 **delegatedAdminServiceManagementDetail** 对象及其属性的列表。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|托管服务的标识符。 只读。|
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
