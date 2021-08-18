---
title: androidEnrollmentCompanyCode 资源类型
description: 用于保留通过 Google 的 Android 管理 API 注册的专用注册数据（如令牌、Url 和 QR 代码内容）的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6803a04883d90d3550b98582522e74465251d96f803896d55e62afff5ad9f58a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54173329"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>androidEnrollmentCompanyCode 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于保留通过 Google 的 Android 管理 API 注册的专用注册数据（如令牌、Url 和 QR 代码内容）的类

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enrollmentToken|字符串|用户用于注册其设备的注册令牌。|
|qrCodeContent|String|用于生成此令牌的 QR 码的字符串。|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|为令牌生成的 QR 代码。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




