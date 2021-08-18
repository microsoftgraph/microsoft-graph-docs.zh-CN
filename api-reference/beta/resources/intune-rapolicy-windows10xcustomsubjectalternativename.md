---
title: windows10XCustomSubjectAlternativeName 资源类型
description: 'SCEP 或 PFX 创建 (身份验证证书的基本配置文件) '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6a16c0e092e89f0e68988d30999ebfd0f24fb1f9fb2f73dd66fdfcd563dc8d35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164123"
---
# <a name="windows10xcustomsubjectalternativename-resource-type"></a>windows10XCustomSubjectAlternativeName 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

SCEP 或 PFX 创建 (身份验证证书的基本配置文件) 

## <a name="properties"></a>属性
|属性|类型|说明|
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




