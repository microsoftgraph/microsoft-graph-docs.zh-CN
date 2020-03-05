---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bfe4139f76e5079475e99c4d529adc59007ba682
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525129"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置管理器客户端状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|配置管理器代理早于1806或未安装，或者此设备未签入 Intune 的30天。|
|了|1 |配置管理器代理已安装，但可能尚未在 configuration manager 控制台中显示。 请等待几小时，让其刷新。|
|运转|7 |此设备能够成功签入 configuration manager 服务。|
|installFailed|8 |配置管理器代理安装失败。|
|updateFailed|11 |从版本 x 更新到配置管理器代理版本 y 的更新失败。 |
|communicationError|合|Configuration manager 代理在过去能够到达 configuration manager 服务，但现在无法再访问。 |



