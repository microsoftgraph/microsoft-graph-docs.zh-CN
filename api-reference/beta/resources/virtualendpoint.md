---
title: virtualEndpoint 资源类型
description: VirtualEndpoint 资源表示云 PC 管理功能的容器。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 168a6f35a3d758911913422f96ea5dc070d57a47
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378292"
---
# <a name="virtualendpoint-resource-type"></a>virtualEndpoint 资源类型

命名空间：microsoft.graph

VirtualEndpoint 资源表示用于管理云电脑的 Api 容器。

使用云 PC API 为组织中的员工设置和管理虚拟桌面。 将其与 [INTUNE API](../resources/intune-graph-overview.md) 结合使用，以管理物理终结点和虚拟终结点。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[获取有效权限](../api/virtualendpoint-geteffectivepermissions.md)|String collection|查看当前经过身份验证的用户的有效权限。|
|[列出 cloudPCs](../api/virtualendpoint-list-cloudpcs.md)|[cloudPC](../resources/cloudpc.md) 集合|列出 [cloudPC](../resources/cloudpc.md) 对象的属性和关系。|
|[列出 deviceImages](../api/virtualendpoint-list-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|列出 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象的属性和关系。|
|[创建 cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|创建新的 [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 对象。|
|[列出 onPremisesConnections](../api/virtualendpoint-list-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|列出 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性和关系。|
|[创建 cloudPcOnPremisesConnection](../api/virtualendpoint-post-onpremisesconnections.md)|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。|
|[列出 provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|列出 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。|
|[创建 cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|id|字符串|虚拟终结点 id 的唯一标识符。只读。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|cloudPCs|[cloudPC](../resources/cloudpc.md) 集合|云托管虚拟桌面。|
|deviceImages|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) 集合|云电脑上的图像资源。|
|onPremisesConnections|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 集合|可用于为云电脑建立本地网络连接的 Azure 资源信息的已定义集合。|
|provisioningPolicies|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|云电脑预配策略。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.virtualEndpoint",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.virtualEndpoint",
  "id": "string"
}
```
