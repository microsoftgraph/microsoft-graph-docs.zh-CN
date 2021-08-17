---
title: iosVppAppAssignedUserLicense 资源类型
description: iOS 批量购买计划用户许可证分配。 此类不支持创建、删除或更新。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7df3d131b8fa932b3cee492736ef33034deb405264f2e4429af8965656a4f22b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54179156"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>iosVppAppAssignedUserLicense 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS 批量购买计划用户许可证分配。 此类不支持创建、删除或更新。


继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 集合|列出 [iosVppAppAssignedUserLicense 对象的属性和](../resources/intune-apps-iosvppappassigneduserlicense.md) 关系。|
|[获取 iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|读取 [iosVppAppAssignedUserLicense 对象的属性和](../resources/intune-apps-iosvppappassigneduserlicense.md) 关系。|
|[创建 iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|创建新的 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象。|
|[删除 iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|无|删除 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)。|
|[更新 iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|更新 [iosVppAppAssignedUserLicense 对象](../resources/intune-apps-iosvppappassigneduserlicense.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|字符串|用户电子邮件地址。 继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|字符串|用户 ID。 继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|用户名。 继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|用户主体名称。 继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```




