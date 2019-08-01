---
title: windowsInformationProtectionDataRecoveryCertificate 资源类型
description: Windows 信息保护 DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 555cac098d2796f612054f11e2c5ade525ad6199
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037728"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>windowsInformationProtectionDataRecoveryCertificate 资源类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 信息保护 DataRecoveryCertificate

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|SubjectName|String|数据恢复证书主题名称|
|说明|String|数据恢复证书说明|
|expirationDateTime|DateTimeOffset|数据恢复证书过期日期/时间|
|证书|Binary|数据恢复证书|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



