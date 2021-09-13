---
title: groupPolicyConfigurationType 枚举类型
description: 组策略配置类型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4a7045e5cf4322f8e4d0c36035b8da7b6a752797
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017336"
---
# <a name="grouppolicyconfigurationtype-enum-type"></a>groupPolicyConfigurationType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略配置类型

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|策略|0|策略类型不会设置该值，这意味着该值将被删除，从而允许使用原始配置值。 策略类型将取代应用程序配置设置，以便应用程序始终知道该值。 策略类型阻止用户通过应用程序的用户界面修改值。|
|preference|1|首选项类型不会使该值小，这意味着不会从注册表中删除该值。 首选项类型将覆盖用户配置的值，并且不会保留以前的值。 首选项类型不会阻止用户通过应用程序的用户界面修改值。|



