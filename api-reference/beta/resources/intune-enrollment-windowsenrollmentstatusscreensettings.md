---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22f7497fb79921bbbf34c6f3334ccc2ae4d7d53
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994900"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册状态屏幕设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hideInstallationProgress|Boolean|显示或隐藏用户的安装进度|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|在配置文件和应用安装完成之前允许或阻止用户使用设备|
|blockDeviceSetupRetryByUser|Boolean|允许用户在安装失败时重试安装程序|
|allowLogCollectionOnInstallFailure|Boolean|在安装失败时允许或阻止日志集合|
|customErrorMessage|String|设置自定义错误消息以在安装失败时显示|
|installProgressTimeoutInMinutes|Int32|设置安装进度超时 (分钟)|
|allowDeviceUseOnInstallFailure|Boolean|允许用户在安装失败时继续使用设备|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





