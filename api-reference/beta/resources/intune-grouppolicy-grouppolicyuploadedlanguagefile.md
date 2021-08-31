---
title: groupPolicyUploadedLanguageFile 资源类型
description: 实体表示管理员上载 (XML 文件的 ADML) 模板语言。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 015e2dc7372ecb2cec607b3e7c6a4aab940f5267
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58794088"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>groupPolicyUploadedLanguageFile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示管理员上载 (XML 文件的 ADML) 模板语言。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|fileName|String|已上载的 ADML 文件的文件名。|
|languageCode|String|上载的 ADML 文件的语言代码。|
|content|二进制|上载的 ADML 文件的内容。|
|id|String|实体的键。|
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



