---
title: defenderProtectionType 枚举类型
description: Defender PUA Protection 的可能值
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eee7d078bc8183fc1955ce43815612e059b89bd2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59115532"
---
# <a name="defenderprotectiontype-enum-type"></a>defenderProtectionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Defender PUA Protection 的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|设备默认值，无意图。|
|enable|1|阻止功能。|
|auditMode|2|允许功能，但生成日志。|
|warn|6 |向能够绕过攻击面减少规则阻止的最终用户发送的警告消息。|
|notConfigured|99|未配置。|



