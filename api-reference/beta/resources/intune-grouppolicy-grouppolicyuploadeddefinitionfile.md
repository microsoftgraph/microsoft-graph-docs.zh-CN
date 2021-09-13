---
title: groupPolicyUploadedDefinitionFile 资源类型
description: 实体表示管理员上载 (XML) ADMX 管理模板。 ADMX 文件包含按类别路径分组策略定义及其位置的集合。 组策略定义文件还包含受支持的语言，这些语言由与语言相关的 ADML 或管理 (模板) 语言文件。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0526b1c2dc11bea9154dc2b2bee519d64671e6a9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030240"
---
# <a name="grouppolicyuploadeddefinitionfile-resource-type"></a>groupPolicyUploadedDefinitionFile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示管理员上载 (XML) ADMX 管理模板。 ADMX 文件包含按类别路径分组策略定义及其位置的集合。 组策略定义文件还包含受支持的语言，这些语言由与语言相关的 ADML 或管理 (模板) 语言文件。


继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyUploadedDefinitionFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-list.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 集合|列出 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象的属性和关系。|
|[获取 groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-get.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|读取 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象的属性和关系。|
|[创建 groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-create.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|创建新的 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 对象。|
|[删除 groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-delete.md)|无|删除 [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)。|
|[更新 groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-update.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|更新 [groupPolicyUploadedDefinitionFile 对象](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) 的属性。|
|[addLanguageFiles 操作](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-addlanguagefiles.md)|无|尚未记录|
|[removeLanguageFiles 操作](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-removelanguagefiles.md)|无|尚未记录|
|[updateLanguageFiles 操作](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-updatelanguagefiles.md)|无|尚未记录|
|[uploadNewVersion 操作](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-uploadnewversion.md)|无|尚未记录|
|[删除操作](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-remove.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|ADMX 文件的本地化友好名称。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|说明|String|ADMX 文件中策略设置的本地化说明。 默认值为空白。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|languageCodes|String collection|ADMX 文件支持的语言代码。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetPrefix|String|指定引用 ADMX 文件内的命名空间的逻辑名称。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetNamespace|String|指定用于标识 ADMX 文件内的命名空间的 URI。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)。 可取值为：`admxBacked`、`admxIngested`。|
|revision|String|与文件关联的修订版本。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|String|实体的键。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|已上载的 ADML 文件的文件名。|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|已上载的 ADMX 文件的上载状态。 可取值为：`none`、`uploadInProgress`、`available`、`assigned`、`removalInProgress`、`uploadFailed` 或 `removalFailed`。|
|content|二进制|上载的 ADMX 文件的内容。|
|uploadDateTime|DateTimeOffset|上传的 ADMX 文件的上传时间。|
|defaultLanguageCode|String|上载的 ADMX 文件的默认语言。|
|groupPolicyUploadedLanguageFiles|[groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md) 集合|与上载的 ADMX 文件关联的 ADML 文件列表。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|定义|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 集合|与文件关联的组策略定义。 继承自 [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|groupPolicyOperations|[groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md) 集合|对已上载的 ADMX 文件的操作列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
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
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
  "status": "String",
  "content": "binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "String",
      "languageCode": "String",
      "content": "binary",
      "id": "String",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```



