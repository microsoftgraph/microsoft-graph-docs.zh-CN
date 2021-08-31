---
title: mobileContainedApp 资源类型
description: 一个抽象类，表示作为包的 mobileApp 中的已包含应用。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c5eb1f5e94ec45d6da289529f2982cd3cbab23c7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787636"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个抽象类，表示作为包的 mobileApp 中的已包含应用。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 集合|列出 [mobileContainedApp 对象的属性和](../resources/intune-apps-mobilecontainedapp.md) 关系。|
|[获取 mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|读取 [mobileContainedApp 对象的属性和](../resources/intune-apps-mobilecontainedapp.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```



