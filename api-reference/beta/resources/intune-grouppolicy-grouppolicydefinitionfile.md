---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示管理模板 (XML) ADMX。 ADMX 文件包含按类别路径分组策略定义及其位置的集合。 组策略定义文件还包含受支持的语言，这些语言由与语言相关的 ADML 或管理 (模板) 语言文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 887c1b3b8b744e45b265fedff2bd2b5fd767fe4b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796192"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>groupPolicyDefinitionFile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示管理模板 (XML) ADMX。 ADMX 文件包含按类别路径分组策略定义及其位置的集合。 组策略定义文件还包含受支持的语言，这些语言由与语言相关的 ADML 或管理 (模板) 语言文件。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|读取 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) 对象的属性和关系。|
|[更新 groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|更新 [groupPolicyDefinitionFile 对象](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|ADMX 文件的本地化友好名称。|
|description|String|ADMX 文件中策略设置的本地化说明。 默认值为空白。|
|languageCodes|字符串集合|ADMX 文件支持的语言代码。|
|targetPrefix|字符串|指定引用 ADMX 文件内的命名空间的逻辑名称。|
|targetNamespace|String|指定用于标识 ADMX 文件内的命名空间的 URI。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 可取值为：`admxBacked`、`admxIngested`。|
|revision|String|与文件关联的修订版本。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|定义|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 集合|与文件关联的组策略定义。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



