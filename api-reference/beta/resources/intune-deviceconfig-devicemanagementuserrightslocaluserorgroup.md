---
title: deviceManagementUserRightsLocalUserOrGroup 资源类型
description: 表示一个本地用户或一组用于设置的用户权限的信息。
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303729"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示一个本地用户或一组用于设置的用户权限的信息。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|name|字符串|此本地用户或组的名称。|
|说明|字符串|此本地用户或组的管理员的说明。|
|securityIdentifier|字符串|此本地用户或组的安全标识符 (例如 * 1-5-32-544)。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





