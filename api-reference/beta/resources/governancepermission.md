---
title: governancePermission 资源类型
description: '表示 governanceSubject 对特定 governanceResource 的访问权限。  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547506"
---
# <a name="governancepermission-resource-type"></a>governancePermission 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[governanceSubject](../resources/governancesubject.md)对特定[governanceResource](../resources/governanceresource.md)的访问权限。  


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accessLevel|String|访问级别。 有效值: ``None``、 ``UserRead`` ``AdminRead``、和。 ``AdminReadWrite``|
|isActive|布尔值|指示请求者是否具有访问级别的任何活动角色分配。|
|isEligible|布尔值|指示请求者是否具有访问级别的任何符合条件的角色分配。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
