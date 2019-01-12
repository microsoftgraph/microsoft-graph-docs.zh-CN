---
title: windowsKioskActiveDirectoryGroup 资源类型
description: 用于标识为网亭配置 Azure Directory 组的类
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632396b727448032f198a54b97ba0a46b961abe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955231"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a>windowsKioskActiveDirectoryGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于标识为网亭配置 Azure Directory 组的类

继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|groupName|字符串|将锁定到此网亭配置 AD 组的名称|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





