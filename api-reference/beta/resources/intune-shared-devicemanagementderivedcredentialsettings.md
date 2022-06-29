---
title: deviceManagementDerivedCredentialSettings 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdc3288d61b141b3a645152a624646dd9a5687fb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441746"
---
# <a name="devicemanagementderivedcredentialsettings-resource-type"></a>deviceManagementDerivedCredentialSettings 资源类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

deviceManagementDerivedCredentialSettings 资源表示一个容器，其内容因工作流而异，包括：  

- 设备配置设置
- RA 策略

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagementDerivedCredentialSettings](../api/intune-shared-devicemanagementderivedcredentialsettings-get.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|读取 [deviceManagementDerivedCredentialSettings 对象的](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 属性和关系。|
|[更新 deviceManagementDerivedCredentialSettings](../api/intune-shared-devicemanagementderivedcredentialsettings-update.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)|更新 [deviceManagementDerivedCredentialSettings 对象的](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 属性。|
|**资源访问策略**|
|[列出 deviceManagementDerivedCredentialSettingses](../api/intune-shared-devicemanagementderivedcredentialsettings-list.md)|[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 集合|列出 [deviceManagementDerivedCredentialSettings 对象的](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 属性和关系。|
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



