---
title: managedAppPhoneNumberRedirectLevel 枚举类型
description: 允许单击打开电话号码、进行电话呼叫或发送短信的应用类。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 21d13f05d3ef5116772803e92852e0128bec8c9e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075030"
---
# <a name="managedappphonenumberredirectlevel-enum-type"></a>managedAppPhoneNumberRedirectLevel 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

允许单击打开电话号码、进行电话呼叫或发送短信的应用类。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|允许所有应用共享。|
|managedApps|1|允许所有托管应用共享。|
|customApp|2|允许对自定义应用共享。|
|blocked|3|阻止应用之间的共享。|



