---
title: androidEnrollmentCompanyCode 资源类型
description: 用于容纳专业注册数据用于注册通过 Google Android 管理 API，如令牌、 Url 和 QR 代码内容的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be5b2a94445e95fe18271467b6661320d8204d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429313"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>androidEnrollmentCompanyCode 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于容纳专业注册数据用于注册通过 Google Android 管理 API，如令牌、 Url 和 QR 代码内容的类

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enrollmentToken|String|注册用户用于注册其设备令牌。|
|qrCodeContent|String|用于生成此令牌的 QR 码的字符串。|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|生成的令牌 QR 代码。|

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




