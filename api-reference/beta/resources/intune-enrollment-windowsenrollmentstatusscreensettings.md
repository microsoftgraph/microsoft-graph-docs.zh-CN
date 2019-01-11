---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7263fdd8ab3d9a39d5081322c62cfcf76a4c7aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877446"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

注册状态屏幕设置
## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|hideInstallationProgress|布尔|显示或隐藏用户安装进度|
|allowDeviceUseBeforeProfileAndAppInstallComplete|布尔|允许或阻止用户使用配置文件和应用程序安装完成之前的设备|
|blockDeviceSetupRetryByUser|布尔|允许用户重试上安装失败的设置|
|allowLogCollectionOnInstallFailure|布尔|允许或阻止上安装失败日志集合|
|customErrorMessage|字符串|设置要在安装失败时显示自定义错误消息|
|installProgressTimeoutInMinutes|Int32|以分钟为单位的设置安装进度超时|
|allowDeviceUseOnInstallFailure|布尔|允许用户继续使用设备上安装失败|

## <a name="relationships"></a>Relationships
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





