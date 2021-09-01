---
title: embeddedSIMDeviceStateValue 枚举类型
description: 介绍嵌入式 SIM 卡激活代码的各种状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ab8db5b259c78ed48a3f1de4a0732dfeb69212d6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785722"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>embeddedSIMDeviceStateValue 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

介绍嵌入式 SIM 卡激活代码的各种状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notEvaluated|0|指定嵌入式 SIM 卡激活代码是免费的，并可以分配给设备。|
|failed|1|指定 Intune 服务无法向设备传递此配置文件。|
|安装|2|指定嵌入的 SIM 卡激活代码已分配给设备，并且设备正在安装令牌。|
|已安装|3|指定已在目标设备上成功安装嵌入式 SIM 卡激活代码。|
|删除|4 |指定 Intune 服务正在尝试从设备中删除配置文件。|
|error|5 |指定此配置文件出错。|
|deleted|6 |指定从设备中删除配置文件。|
|removedByUser|7 |指定用户从设备中删除配置文件|



