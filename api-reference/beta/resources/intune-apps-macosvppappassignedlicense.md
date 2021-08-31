---
title: macOsVppAppAssignedLicense 资源类型
description: MacOS 批量购买计划许可证分配。 此类不支持创建、删除或更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 036f3ed99dd9af00c5e663f5236817d041785f30
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789704"
---
# <a name="macosvppappassignedlicense-resource-type"></a>macOsVppAppAssignedLicense 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 批量购买计划许可证分配。 此类不支持创建、删除或更新。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 集合|列出 [macOsVppAppAssignedLicense 对象的属性和](../resources/intune-apps-macosvppappassignedlicense.md) 关系。|
|[获取 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|读取 [macOsVppAppAssignedLicense 对象的属性和](../resources/intune-apps-macosvppappassignedlicense.md) 关系。|
|[创建 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|创建新的 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象。|
|[删除 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-delete.md)|无|删除 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)。|
|[更新 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|更新 [macOsVppAppAssignedLicense 对象](../resources/intune-apps-macosvppappassignedlicense.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userEmailAddress|String|用户电子邮件地址。|
|userId|String|用户 ID。|
|userName|String|用户名。|
|userPrincipalName|String|用户主体名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOsVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```



