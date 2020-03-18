---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 38e0eaef1fb4f76584fc791d0b5847832f186dbf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783100"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|policy|0|策略类型不 tattoo 值，这意味着将删除值，允许使用原始配置值。 策略类型取代应用程序配置设置，以便应用程序始终知道该值。 策略类型可阻止用户通过应用程序的用户界面修改值。|
|优先权|1|首选项类型不 tattoo 值，这意味着不会从注册表中删除该值。 首选项类型将覆盖用户配置的值，并且不会保留以前的值。 首选类型不阻止用户通过应用程序的用户界面修改值。|



