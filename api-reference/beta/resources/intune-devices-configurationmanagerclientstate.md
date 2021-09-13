---
title: configurationManagerClientState 枚举类型
description: 配置管理器客户端状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7c2080ba9713c00942dbf59487292f6d3b366e20
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59026943"
---
# <a name="configurationmanagerclientstate-enum-type"></a>configurationManagerClientState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

配置管理器客户端状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|配置管理器代理超过 1806 年或者未安装，或者此设备在 30 天内未签入 Intune。|
|已安装|1|配置管理器代理已安装，但可能尚未显示在配置管理器控制台中。 请等待几小时，等待刷新。|
|healthy|7 |此设备能够成功签入配置管理器服务。|
|installFailed|8 |配置管理器代理安装失败。|
|updateFailed|11|配置管理器代理从版本 x 更新到版本 y 失败。 |
|communicationError|19|配置管理器代理过去能够访问配置管理器服务，但现在无法再访问。 |



