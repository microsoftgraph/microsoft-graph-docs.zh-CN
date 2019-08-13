---
title: mobileContainedApp 资源类型
description: 一个抽象类, 表示充当包的 mobileApp 中包含的应用程序。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f0c20b73c753ea4d51e18469f97841b02e01e83
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331775"
---
# <a name="mobilecontainedapp-resource-type"></a>mobileContainedApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个抽象类, 表示充当包的 mobileApp 中包含的应用程序。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合|列出[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的属性和关系。|
|[获取 mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|读取[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的属性和关系。|

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



