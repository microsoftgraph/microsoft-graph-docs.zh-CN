---
title: groupPolicyDefinitionFile 资源类型
description: 实体表示 ADMX （管理模板） XML 文件。 ADMX 文件包含类别路径其位置和组策略定义的集合。 组策略定义文件还包含由语言相关 ADML （管理模板） 语言文件支持的语言。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431351"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>groupPolicyDefinitionFile 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示 ADMX （管理模板） XML 文件。 ADMX 文件包含类别路径其位置和组策略定义的集合。 组策略定义文件还包含由语言相关 ADML （管理模板） 语言文件支持的语言。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|读取属性和[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的关系。|
|[更新 groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|更新[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|ADMX 文件的本地化的友好名称。|
|说明|String|ADMX 文件中的策略设置的本地化的描述。 默认值为空。|
|languageCodes|String 集合|ADMX 文件的受支持的语言代码。|
|targetPrefix|String|指定引用 ADMX 文件中的命名空间的逻辑名称。|
|targetNamespace|String|指定用于标识 ADMX 文件中的命名空间的 URI。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定的组策略的类型。 可取值为：`admxBacked`、`admxIngested`。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|日期和实体上次修改的时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|定义|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)集合|组策略定义与文件关联。|

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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




