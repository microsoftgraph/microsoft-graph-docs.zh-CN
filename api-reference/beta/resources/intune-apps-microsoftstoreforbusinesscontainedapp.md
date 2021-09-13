---
title: microsoftStoreForBusinessContainedApp 资源类型
description: 表示 MicrosoftStoreForBusinessApp 的包含应用的类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b48baf12c4e997ab500722d8f8ac44fefdcc66ce
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59087062"
---
# <a name="microsoftstoreforbusinesscontainedapp-resource-type"></a>microsoftStoreForBusinessContainedApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 MicrosoftStoreForBusinessApp 的包含应用的类。


继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 microsoftStoreForBusinessContainedApps](../api/intune-apps-microsoftstoreforbusinesscontainedapp-list.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 集合|列出 [microsoftStoreForBusinessContainedApp 对象的属性和](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 关系。|
|[获取 microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-get.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|读取 [microsoftStoreForBusinessContainedApp 对象的属性和](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 关系。|
|[创建 microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-create.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|创建新的 [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 对象。|
|[删除 microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-delete.md)|无|删除 [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)。|
|[更新 microsoftStoreForBusinessContainedApp](../api/intune-apps-microsoftstoreforbusinesscontainedapp-update.md)|[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)|更新 [microsoftStoreForBusinessContainedApp 对象](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)|
|appUserModelId|String|MicrosoftStoreForBusinessApp 包含的应用程序的应用程序用户模型 ID。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "String (identifier)",
  "appUserModelId": "String"
}
```



