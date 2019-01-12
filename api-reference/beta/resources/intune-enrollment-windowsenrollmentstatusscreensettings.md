---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: abc48a1d63cc514d2ec887a7758e69a0ea8112a7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978569"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

注册状态屏幕设置
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hideInstallationProgress|Boolean|显示或隐藏用户安装进度|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|允许或阻止用户使用配置文件和应用程序安装完成之前的设备|
|blockDeviceSetupRetryByUser|Boolean|允许用户重试上安装失败的设置|
|allowLogCollectionOnInstallFailure|Boolean|允许或阻止上安装失败日志集合|
|customErrorMessage|字符串|设置要在安装失败时显示自定义错误消息|
|installProgressTimeoutInMinutes|Int32|以分钟为单位的设置安装进度超时|
|allowDeviceUseOnInstallFailure|Boolean|允许用户继续使用设备上安装失败|

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





