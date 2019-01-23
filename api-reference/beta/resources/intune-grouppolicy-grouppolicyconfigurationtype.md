---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 372a5bd5656510c43b388bac128cba4bc46c0988
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429410"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|策略|0|策略类型不图案的值，这意味着值删除允许使用的原始配置值。 策略类型取代应用程序配置设置，以便应用程序始终会知道的值。 策略类型可防止用户修改通过应用程序的用户界面的值。|
|preference|1|首选项类型图案的值，这意味着值不从注册表中删除。 首选项类型将覆盖用户配置值并不会保留以前的值。 首选项类型不阻止用户修改通过应用程序的用户界面的值。|




