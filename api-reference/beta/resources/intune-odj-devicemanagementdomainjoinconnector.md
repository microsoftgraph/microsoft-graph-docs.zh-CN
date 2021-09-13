---
title: deviceManagementDomainJoinConnector 资源类型
description: 域加入连接器是一个连接器，负责分配 (和删除) 帐户 blob
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d638537c50c10a9e8a520cd9dc50316e7e3e3f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017273"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a>deviceManagementDomainJoinConnector 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

域加入连接器是一个连接器，负责分配 (和删除) 帐户 blob

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementDomainJoinConnectors](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 集合|列出 [deviceManagementDomainJoinConnector 对象的属性和](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 关系。|
|[获取 deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|读取 [deviceManagementDomainJoinConnector 对象的属性和](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 关系。|
|[创建 deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|创建新的 [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 对象。|
|[删除 deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|None|删除 [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)。|
|[更新 deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|更新 [deviceManagementDomainJoinConnector 对象](../resources/intune-odj-devicemanagementdomainjoinconnector.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|表示连接器的唯一标识符。|
|displayName|String|连接器显示名称。|
|lastConnectionDateTime|DateTimeOffset|上次连接器与 Intune 联系的时间。|
|state|[deviceManagementDomainJoinConnectorState](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|连接器状态。 可取值为：`active`、`error`、`inactive`。|
|version|String|连接器的版本。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```



