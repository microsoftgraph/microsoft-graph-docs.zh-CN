---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18c947bbfc7e11ba4acef967171f77a7806b3509
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772795"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册状态屏幕设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hideInstallationProgress|布尔值|显示或隐藏用户的安装进度|
|allowDeviceUseBeforeProfileAndAppInstallComplete|布尔值|在配置文件和应用安装完成之前允许或阻止用户使用设备|
|blockDeviceSetupRetryByUser|布尔值|允许用户在安装失败时重试安装程序|
|allowLogCollectionOnInstallFailure|布尔值|在安装失败时允许或阻止日志集合|
|customErrorMessage|String|设置自定义错误消息以在安装失败时显示|
|installProgressTimeoutInMinutes|Int32|设置安装进度超时 (分钟)|
|allowDeviceUseOnInstallFailure|布尔值|允许用户在安装失败时继续使用设备|

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





