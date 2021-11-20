---
title: cloudPcServicePlan 资源类型
description: 表示Windows云电脑配置的所有 365 服务计划。
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 281bfdbaefde3b58b8bb9c0367d92d7dfc0bebb3
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2021
ms.locfileid: "61123949"
---
# <a name="cloudpcserviceplan-resource-type"></a>cloudPcServicePlan 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Windows云电脑配置的所有 365 服务计划。

有关当前可用的服务计划的示例，请参阅[Windows 365 比较计划和定价](https://www.microsoft.com/windows-365/business/compare-plans-pricing)。 目前，microsoft Graph API 可用于 Windows 365 Enterprise。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[List servicePlans](../api/virtualendpoint-list-serviceplans.md)|[cloudPcServicePlan](../resources/cloudpcserviceplan.md) 集合|列出组织可购买云电脑当前可用的服务计划。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|服务计划的名称。 只读。|
|id|String|服务计划的唯一标识符。 只读。|
|ramInGB|Int32|RAM 的大小（以 GB 为单位）。 只读。|
|storageInGB|Int32|操作系统磁盘的大小（以 GB 为单位）。 只读。|
|类型|[cloudPcServicePlanType](#cloudpcserviceplantype-values)|服务计划的类型。 可取值为：`enterprise`、`business`、`unknownFutureValue`。 只读。|
|userProfileInGB|Int32|用户配置文件磁盘的大小（以 GB 为单位）。 只读。|
|vCpuCount|Int32|vCPUs 的数量。 只读。|

### <a name="cloudpcserviceplantype-values"></a>cloudPcServicePlanType 值

|成员|说明|
|:---|:---|
|enterprise|Enterprise客户的服务计划类型。|
|business|针对小型企业或 VSB 客户的业务服务 () 类型。|
|unknownFutureValue|可发展枚举 sentinel 值。 请勿使用。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcServicePlan",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcServicePlan",
  "id": "String (identifier)",
  "displayName": "String",
  "type": "String",
  "vCpuCount": "Int32",
  "ramInGB": "Int32",
  "storageInGB": "Int32",
  "userProfileInGB": "Int32"
}
```
