---
title: deviceRegistrationState 枚举类型
description: 设备注册状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bc19571455456b80516259deba413cc69d203388
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125853"
---
# <a name="deviceregistrationstate-enum-type"></a>deviceRegistrationState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备注册状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notRegistered|0|设备未注册。|
|registered|2|设备已注册。|
|revoked|3|设备已被阻止、擦除或停用。|
|keyConflict|4 |设备存在密钥冲突。|
|approvalPending|5 |设备正在等待审批。|
|certificateReset|6 |设备证书已重置。|
|notRegisteredPendingEnrollment|7 |设备未注册，正在等待注册。|
|unknown|8 |设备注册状态未知。|



