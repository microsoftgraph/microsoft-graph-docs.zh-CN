---
title: windowsInformationProtectionAppLockerFile 资源类型
description: Windows 信息保护 AppLocker 文件
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eb03faef97edad7446595b985e9e3db545ef420f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415115"
---
# <a name="windowsinformationprotectionapplockerfile-resource-type"></a>windowsInformationProtectionAppLockerFile 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 信息保护 AppLocker 文件

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 windowsInformationProtectionAppLockerFiles](../api/intune-mam-windowsinformationprotectionapplockerfile-list.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 集合|列出 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性和关系。|
|[获取 windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-get.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|读取 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性和关系。|
|[创建 windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-create.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|创建新的 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。|
|[删除 windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-delete.md)|无|删除 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)。|
|[更新 windowsInformationProtectionAppLockerFile](../api/intune-mam-windowsinformationprotectionapplockerfile-update.md)|[windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)|更新 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|友好名称|
|fileHash|String|文件的 SHA256 哈希|
|file|Binary|字节数组形式的文件|
|id|String|实体的键。|
|version|String|实体的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionAppLockerFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "String",
  "fileHash": "String",
  "file": "binary",
  "id": "String (identifier)",
  "version": "String"
}
```




