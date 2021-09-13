---
title: remoteAssistanceState 枚举类型
description: 帐户的远程协助状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ee67be86f9b3144ba8a002814637939f4fe7bdc4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039474"
---
# <a name="remoteassistancestate-enum-type"></a>remoteAssistanceState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

帐户的远程协助状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未为帐户配置远程协助。 使用此值，快速助手远程协助功能。|
|disabled|1|对帐户禁用远程协助。 使用此值，快速助手帐户不允许远程协助会话。|
|enabled|2|为帐户启用远程协助。 使用此值，快速助手远程协助功能。|



