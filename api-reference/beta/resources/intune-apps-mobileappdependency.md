---
title: mobileAppDependency 资源类型
description: 描述两个移动应用之间的依赖关系类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a29f658a67c3930b1b693589dc9115c0c1ff185
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990258"
---
# <a name="mobileappdependency-resource-type"></a>mobileAppDependency 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

描述两个移动应用之间的依赖关系类型。


继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppDependencies](../api/intune-apps-mobileappdependency-list.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)集合|列出[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。|
|[获取 mobileAppDependency](../api/intune-apps-mobileappdependency-get.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|读取[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性和关系。|
|[创建 mobileAppDependency](../api/intune-apps-mobileappdependency-create.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。|
|[删除 mobileAppDependency](../api/intune-apps-mobileappdependency-delete.md)|无|删除[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)。|
|[更新 mobileAppDependency](../api/intune-apps-mobileappdependency-update.md)|[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)|更新[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|目标子移动应用程序的显示名称。 继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|dependencyType|[mobileAppDependencyType](../resources/intune-apps-mobileappdependencytype.md)|父应用和子应用之间的依赖关系的类型。 可取值为：`detect`、`autoInstall`。|
|dependentAppCount|Int32|子应用程序的依赖项总数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppDependency"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "String (identifier)",
  "targetId": "String",
  "targetDisplayName": "String",
  "dependencyType": "String",
  "dependentAppCount": 1024
}
```





