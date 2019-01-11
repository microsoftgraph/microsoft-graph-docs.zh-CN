---
title: mobileAppContent 资源类型
description: 包含特定应用版本的内容属性。 每个 mobileAppContent 都可以具有多个 mobileAppContentFile。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: aa68d0a07de4f0e85ee15acc189e003c4f4120a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845813"
---
# <a name="mobileappcontent-resource-type"></a>mobileAppContent 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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





