---
title: officeConfiguration 资源类型
description: 充当所有设备管理功能的容器的单例实体。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58e1aea2e6b8a03f69e63948675e4f4b7a9b6ebf
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820525"
---
# <a name="officeconfiguration-resource-type"></a>officeConfiguration 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

充当所有设备管理功能的容器的单例实体。

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|获取 officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|读取 [officeConfiguration 对象的属性和](../resources/intune-cirrus-officeconfiguration.md) 关系。|
|更新 officeConfiguration|[officeConfiguration](../resources/intune-cirrus-officeconfiguration.md)|更新 [officeConfiguration 对象](../resources/intune-cirrus-officeconfiguration.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Office 配置的 ID。|
|tenantCheckinStatuses|[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) 集合|Office 客户端签入状态列表。|
|tenantUserCheckinSummary|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|描述租户签入计划的实体|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|clientConfigurations|[officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md) 集合|Office 客户端配置列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "String (identifier)",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "String",
      "deviceName": "String",
      "devicePlatform": "String",
      "devicePlatformVersion": "String",
      "wasSuccessful": true,
      "userId": "String",
      "checkinDateTime": "String (timestamp)",
      "errorMessage": "String",
      "appliedPolicies": [
        "String"
      ]
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 1024,
    "failedUserCount": 1024
  }
}
```



