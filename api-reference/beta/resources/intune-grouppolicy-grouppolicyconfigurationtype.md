---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0d3a0daa73fef30e5425e188958bdc54e61778d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164685"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|policy|0|策略类型不 tattoo 值, 这意味着将删除值, 允许使用原始配置值。 策略类型取代应用程序配置设置, 以便应用程序始终知道该值。 策略类型可阻止用户通过应用程序的用户界面修改值。|
|preference|1|首选项类型不 tattoo 值, 这意味着不会从注册表中删除该值。 首选项类型将覆盖用户配置的值, 并且不会保留以前的值。 首选类型不阻止用户通过应用程序的用户界面修改值。|




