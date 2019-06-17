---
title: customSubjectAlternativeName 资源类型
description: 自定义主题备用名称定义
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5c00361a62315f250c0f839338f5e7a3fe3914c3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979975"
---
# <a name="customsubjectalternativename-resource-type"></a>customSubjectAlternativeName 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自定义主题备用名称定义

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|sanType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|自定义 SAN 类型。 可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`。|
|name|String|自定义 SAN 名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





