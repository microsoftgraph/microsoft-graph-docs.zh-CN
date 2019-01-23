---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ceeb6cd4e989f4e020c885dde119c39d9659539c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418181"
---
# <a name="mobileappcontent-resource-type"></a>mobileAppContent 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileAppContents](../api/intune-apps-mobileappcontent-list.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md) 集合|列出 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。|
|[获取 mobileAppContent](../api/intune-apps-mobileappcontent-get.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|读取 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性和关系。|
|[创建 mobileAppContent](../api/intune-apps-mobileappcontent-create.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。|
|[删除 mobileAppContent](../api/intune-apps-mobileappcontent-delete.md)|无|删除 [mobileAppContent](../resources/intune-apps-mobileappcontent.md)。|
|[更新 mobileAppContent](../api/intune-apps-mobileappcontent-update.md)|[mobileAppContent](../resources/intune-apps-mobileappcontent.md)|更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|应用内容版本。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|files|[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 集合|此应用内容版本的文件列表。|
|containedApps|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合|包含充当包 MobileLobApp 中的应用程序的集合。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```




