---
title: iosVppAppAssignedLicense 资源类型
description: iOS 卷购买计划许可证分配。 此类不支持创建、删除或更新。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5d2588cd8ceeae44b7e4150544a984c68d4d90e3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991210"
---
# <a name="iosvppappassignedlicense-resource-type"></a>iosVppAppAssignedLicense 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

iOS 卷购买计划许可证分配。 此类不支持创建、删除或更新。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)集合|列出属性和[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象之间的关系。|
|[获取 iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|读取属性和[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的关系。|
|[创建 iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|创建新的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象。|
|[删除 iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|无|删除[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)。|
|[更新 iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|更新[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userEmailAddress|字符串|用户电子邮件地址。|
|userId|String|用户 id。|
|userName|String|用户名。|
|userPrincipalName|字符串|用户主体名称。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





