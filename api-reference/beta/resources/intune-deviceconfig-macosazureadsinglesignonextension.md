---
title: macOSAzureAdSingleSignOnExtension 资源类型
description: 表示 macOS 设备的 Azure AD 类型单一登录扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b70a34c8a664ea47804bc5517a419211a8938a96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084987"
---
# <a name="macosazureadsinglesignonextension-resource-type"></a>macOSAzureAdSingleSignOnExtension 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 设备的 Azure AD 类型单一登录扩展配置文件。


继承自 [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enableSharedDeviceMode|布尔|启用或禁用共享设备模式。|
|bundleIdAccessControlList|字符串集合|允许为单一登录使用 AAD 扩展的附加捆绑捆绑 Id 的可选列表。|
|配置|[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) 集合|获取或设置用于配置凭据类型配置文件的类型键/值对的列表。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```






