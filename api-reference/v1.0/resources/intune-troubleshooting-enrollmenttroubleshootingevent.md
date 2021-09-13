---
title: enrollmentTroubleshootingEvent 资源类型
description: 表示注册失败的事件。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1812a0aa6501735a737752c3ab58a2b7aa7daab6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021524"
---
# <a name="enrollmenttroubleshootingevent-resource-type"></a>enrollmentTroubleshootingEvent 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示注册失败的事件。


继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 enrollmentTroubleshootingEvents](../api/intune-troubleshooting-enrollmenttroubleshootingevent-list.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 集合|列出 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。|
|[获取 enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-get.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|读取 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性和关系。|
|[创建 enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-create.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|创建新的 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象。|
|[删除 enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-delete.md)|无|删除 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)。|
|[更新 enrollmentTroubleshootingEvent](../api/intune-troubleshooting-enrollmenttroubleshootingevent-update.md)|[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md)|更新 [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 UUID。继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|事件发生的时间。 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|correlationId|String|用于跟踪服务中的故障的 ID。 继承自 [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|String|Intune 创建或收集的设备标识符。|
|operatingSystem|String|操作系统。|
|osVersion|String|操作系统版本。|
|userId|String|尝试注册设备的用户的标识符。|
|deviceId|String|Azure AD 设备标识符。|
|enrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|注册类型。 可能的值是：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`、`windowsAzureADJoinUsingDeviceAuth`、`appleUserEnrollment`、`appleUserEnrollmentWithServiceAccount`。|
|failureCategory|[deviceEnrollmentFailureReason](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|Highlevel 失败类别。 可取值为：`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment`。|
|failureReason|String|详细失败原因。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```




