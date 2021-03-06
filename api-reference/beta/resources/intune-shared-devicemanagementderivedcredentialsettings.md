---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 260412a844bfa17c485e646e0b9feddbb628c5e3
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866872"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a>deviceManagementDerivedCredentialSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

deviceManagementDerivedCredentialSettings 资源表示其内容因工作流而异的容器，包括：  

- 设备配置设置
- RA 策略

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagementDerivedCredentialSettings](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|读取 [deviceManagementDerivedCredentialSettings 对象的属性和](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 关系。|
|[更新 deviceManagementDerivedCredentialSettings](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|更新 [deviceManagementDerivedCredentialSettings 对象](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 的属性。|
|**资源访问策略**|
|[列出 deviceManagementDerivedCredentialSettingses](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 集合|列出 [deviceManagementDerivedCredentialSettings 对象的属性和](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 关系。|
[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|创建新的 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象。|
|[删除 deviceManagementDerivedCredentialSettings](../api/intune-shared-devicemanagementderivedcredentialsettings-delete.md)|无|删除 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|派生凭据的唯一标识符|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDerivedCredentialSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "String (identifier)"
}
```




