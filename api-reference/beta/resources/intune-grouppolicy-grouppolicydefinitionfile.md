---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示 ADMX (管理模板) XML 文件。 ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。 组策略定义文件还包含由语言相关 ADML (管理模板) 语言文件所确定的受支持的语言。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 384b59a2c9e1b669cd71b294c6420c13b95d1102
ms.sourcegitcommit: 705b32b9a64516d8138fab34c173b7df4f78a6ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/05/2019
ms.locfileid: "35576485"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>groupPolicyDefinitionFile 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示 ADMX (管理模板) XML 文件。 ADMX 文件包含组策略定义的集合及其在各类别路径中的位置。 组策略定义文件还包含由语言相关 ADML (管理模板) 语言文件所确定的受支持的语言。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|读取[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性和关系。|
|[更新 groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|ADMX 文件的本地化友好名称。|
|说明|String|ADMX 文件中策略设置的本地化说明。 默认值为空白。|
|languageCodes|String collection|ADMX 文件的受支持的语言代码。|
|targetPrefix|String|指定在 ADMX 文件中引用命名空间的逻辑名称。|
|targetNamespace|String|指定用于标识 ADMX 文件中的命名空间的 URI。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 可取值为：`admxBacked`、`admxIngested`。|
|a01|String|与文件关联的修订版本。|
|id|字符串|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|限定|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合|与文件相关联的组策略定义。|

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



