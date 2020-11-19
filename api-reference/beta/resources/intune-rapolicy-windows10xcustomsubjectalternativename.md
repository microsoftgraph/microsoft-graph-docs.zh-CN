---
title: windows10XCustomSubjectAlternativeName 资源类型
description: " (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 725d2cc13db1cb28b9286479f201b9bb38f6eefa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301503"
---
# <a name="windows10xcustomsubjectalternativename-resource-type"></a>windows10XCustomSubjectAlternativeName 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

 (SCEP 或 PFX Create) 的身份验证证书的基本配置文件类型

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|sanType|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|自定义 SAN 类型。 可取值为：`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService`、`universalResourceIdentifier`。|
|name|String|自定义 SAN 名称|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCustomSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




