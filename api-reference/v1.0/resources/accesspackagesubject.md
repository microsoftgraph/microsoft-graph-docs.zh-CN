---
title: accessPackageSubject 资源类型
description: 在Azure AD权限管理中，访问包分配的主题。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d22ab7f69213625468b1cb5857a47147fbdd7889
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242356"
---
# <a name="accesspackagesubject-resource-type"></a>accessPackageSubject 资源类型

命名空间：microsoft.graph


在[Azure AD中](entitlementmanagement-root.md)，访问包主题是可配置为请求或分配访问包的用户、服务主体或其他实体。  它可以表示来自尚未在租户中的已连接组织的请求者。

## <a name="methods"></a>方法

无。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|主题显示名称。|
|email|String|主题的电子邮件地址。|
|id|String|只读。|
|objectId|String|主题的对象标识符。 `null` 如果主题不是租户中的用户。|
|onPremisesSecurityIdentifier|String|主体的安全标识符（如果已知）或主题没有安全标识符的 `null` 字符串表示形式。|
|principalName|String|主题的主体名称（如果已知）。|
|subjectType|accessPackageSubjectType|主题的资源类型。 可能的值包括 `notSpecified`、`user`、`servicePrincipal`、`unknownFutureValue`。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|connectedOrganization|[connectedOrganization](connectedorganization.md)|主题的已连接组织。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageSubject",
  "id": "String (identifier)",
  "objectId": "String",
  "onPremisesSecurityIdentifier": "String",
  "displayName": "String",
  "principalName": "String",
  "email": "String",
  "subjectType": "String"
}
```

