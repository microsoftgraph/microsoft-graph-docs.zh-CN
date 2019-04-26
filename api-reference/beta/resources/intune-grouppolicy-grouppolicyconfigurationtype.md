---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e520bdac154ad418cd56a7984eff71ab925984d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564027"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|策略|0|策略类型不 tattoo 值, 这意味着将删除值, 允许使用原始配置值。 策略类型取代应用程序配置设置, 以便应用程序始终知道该值。 策略类型可阻止用户通过应用程序的用户界面修改值。|
|优先权|1|首选项类型不 tattoo 值, 这意味着不会从注册表中删除该值。 首选项类型将覆盖用户配置的值, 并且不会保留以前的值。 首选类型不阻止用户通过应用程序的用户界面修改值。|





