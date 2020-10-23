---
title: macOsVppAppAssignedLicense 资源类型
description: MacOS Volume Purchase Program 许可证分配。 此类不支持创建、删除或更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 49c940ee5a79a5e2139806da9754c0e87cee045f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691531"
---
# <a name="macosvppappassignedlicense-resource-type"></a>macOsVppAppAssignedLicense 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS Volume Purchase Program 许可证分配。 此类不支持创建、删除或更新。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 集合|列出 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象的属性和关系。|
|[获取 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|读取 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象的属性和关系。|
|[创建 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|创建新的 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象。|
|[删除 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-delete.md)|无|删除 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)。|
|[更新 macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|更新 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象的属性。|

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





