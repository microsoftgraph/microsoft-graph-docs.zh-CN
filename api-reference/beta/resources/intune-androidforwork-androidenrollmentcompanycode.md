---
title: androidEnrollmentCompanyCode 资源类型
description: 用于保存用于通过 Google 的 Android 管理 API (如令牌、Url 和 QR 代码内容) 进行注册的专业注册数据的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fdbcf69751cf341c78c654580a709b0873213289
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005658"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>androidEnrollmentCompanyCode 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于保存用于通过 Google 的 Android 管理 API (如令牌、Url 和 QR 代码内容) 进行注册的专业注册数据的类

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enrollmentToken|String|用户用于注册其设备的注册令牌。|
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





