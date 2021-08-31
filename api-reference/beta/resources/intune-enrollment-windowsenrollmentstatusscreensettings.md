---
title: windowsEnrollmentStatusScreenSettings 资源类型
description: 注册状态屏幕设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 98de649856d89d0dfaa484a3abcf816463241743
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797238"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a>windowsEnrollmentStatusScreenSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

注册状态屏幕设置

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|hideInstallationProgress|Boolean|向用户显示或隐藏安装进度|
|allowDeviceUseBeforeProfileAndAppInstallComplete|Boolean|在配置文件应用安装完成之前，允许或阻止用户使用设备|
|blockDeviceSetupRetryByUser|Boolean|允许用户在安装失败时重试安装|
|allowLogCollectionOnInstallFailure|Boolean|安装失败时允许或阻止日志收集|
|customErrorMessage|String|将自定义错误消息设置为在安装失败时显示|
|installProgressTimeoutInMinutes|Int32|设置安装进度超时（分钟）|
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



