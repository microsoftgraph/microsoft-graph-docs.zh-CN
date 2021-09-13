---
title: iosAzureAdSingleSignOnExtension 资源类型
description: 表示 iOS 设备的 Azure AD 类型单Sign-On扩展配置文件。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db51aeebee2709af56a248226b7c16e1795f444f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115483"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a>iosAzureAdSingleSignOnExtension 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 iOS 设备的 Azure AD 类型单Sign-On扩展配置文件。


继承自 [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enableSharedDeviceMode|Boolean|启用或禁用共享设备模式。|
|bundleIdAccessControlList|字符串集合|允许将 AAD 扩展用于单一登录的其他捆绑包的可选列表。|
|配置|[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) 集合|获取或设置用于配置凭据类型配置文件的键入键值对的列表。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```



