---
title: windowsUniversalAppXContainedApp 资源类型
description: 表示 WindowsUniversalAppX 应用的包含应用的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3dcdfcbe3bd61b175d9905337131e84b80a8ad82
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091830"
---
# <a name="windowsuniversalappxcontainedapp-resource-type"></a>windowsUniversalAppXContainedApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 WindowsUniversalAppX 应用的包含应用的类。


继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsUniversalAppXContainedApps](../api/intune-apps-windowsuniversalappxcontainedapp-list.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 集合|列出 [windowsUniversalAppXContainedApp 对象的属性和](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 关系。|
|[获取 windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-get.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|读取 [windowsUniversalAppXContainedApp 对象的属性和](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 关系。|
|[创建 windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-create.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|创建新的 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 对象。|
|[删除 windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-delete.md)|无|删除 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)。|
|[更新 windowsUniversalAppXContainedApp](../api/intune-apps-windowsuniversalappxcontainedapp-update.md)|[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)|更新 [windowsUniversalAppXContainedApp 对象](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|String|WindowsUniversalAppX 应用包含的应用的应用用户模型 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppXContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```



