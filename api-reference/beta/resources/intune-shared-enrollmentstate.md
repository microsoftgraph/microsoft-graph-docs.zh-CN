---
title: enrollmentState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: afe74408d7e372b6fd9c92a31afd988bc3457f72
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441130"
---
# <a name="enrollmentstate-enum-type"></a>enrollmentState 枚举类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|设备注册状态未知|
|登记|1|设备已注册。|
|pendingReset|2|已注册，但已通过注册配置文件注册，并且已注册的配置文件与分配的配置文件不同。|
|失败|3|未注册，并且存在注册失败记录。|
|notContacted|4|设备已导入但未注册。|
|封锁|5|设备注册为无用户，但因应用安装失败而被阻止移动到用户注册。|



