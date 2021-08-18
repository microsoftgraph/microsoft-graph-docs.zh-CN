---
title: groupPolicyUploadedLanguageFile 资源类型
description: 实体表示管理员上载 (XML) 一种 ADML 管理模板语言。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c77b9f6fab6bbd1127aff4abc0176a9298f6e6a2955f69a2781c9f22f63069f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54122360"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a>groupPolicyUploadedLanguageFile 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体表示管理员上载 (XML) 一种 ADML 管理模板语言。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|fileName|String|已上载的 ADML 文件的文件名。|
|languageCode|字符串|上载的 ADML 文件的语言代码。|
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




