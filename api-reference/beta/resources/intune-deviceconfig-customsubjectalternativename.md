---
title: customSubjectAlternativeName 资源类型
description: 自定义的 Subject Alternative Name 定义
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3f081b37b79be45d6705d24be58ea7295b58b68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415668"
---
# <a name="customsubjectalternativename-resource-type"></a>customSubjectAlternativeName 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自定义的 Subject Alternative Name 定义

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




