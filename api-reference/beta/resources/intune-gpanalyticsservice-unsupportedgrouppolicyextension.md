---
title: unsupportedGroupPolicyExtension 资源类型
description: 不支持的组策略扩展。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 133a6b5605f7a8efe880eb71d3354ba59623152b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785701"
---
# <a name="unsupportedgrouppolicyextension-resource-type"></a>unsupportedGroupPolicyExtension 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

不支持的组策略扩展。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 unsupportedGroupPolicyExtensions](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-list.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 集合|列出 [unsupportedGroupPolicyExtension 对象的属性和](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 关系。|
|[获取 unsupportedGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-get.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|读取 [unsupportedGroupPolicyExtension 对象的属性和](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 关系。|
|[创建 unsupportedGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-create.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|创建新的 [unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 对象。|
|[删除 unsupportedGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-delete.md)|无|删除不 [受支持的GroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)。|
|[更新 unsupportedGroupPolicyExtension](../api/intune-gpanalyticsservice-unsupportedgrouppolicyextension-update.md)|[unsupportedGroupPolicyExtension](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md)|更新 [unsupportedGroupPolicyExtension 对象](../resources/intune-gpanalyticsservice-unsupportedgrouppolicyextension.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|设置不受支持扩展的作用域。 可取值为：`unknown`、`device`、`user`。|
|namespaceUrl|String|不支持的扩展的命名空间 URL。|
|extensionType|String|不支持的扩展的 ExtensionType。|
|nodeName|String|不受支持扩展的节点名称。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unsupportedGroupPolicyExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedGroupPolicyExtension",
  "id": "String (identifier)",
  "settingScope": "String",
  "namespaceUrl": "String",
  "extensionType": "String",
  "nodeName": "String"
}
```



