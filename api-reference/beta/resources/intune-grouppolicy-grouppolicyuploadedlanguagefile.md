---
title: groupPolicyUploadedLanguageFile 资源类型
description: 实体表示管理员上载的 ADML (管理模板语言) XML 文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf5bef8faadac012df13a8a31cfaac3a5dc94ed2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298104"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>groupPolicyUploadedLanguageFile 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示管理员上载的 ADML (管理模板语言) XML 文件。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|fileName|String|上传的 ADML 文件的文件名。|
|languageCode|字符串|上传的 ADML 文件的语言代码。|
|content|Binary|已上载的 ADML 文件的内容。|
|id|字符串|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedLanguageFile",
  "fileName": "String",
  "languageCode": "String",
  "content": "binary",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




