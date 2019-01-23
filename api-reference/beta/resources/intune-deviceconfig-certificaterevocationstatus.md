---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 373cb6247a695a5912d02d4fb1a353c40aeac581
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421968"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

证书吊销状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未被吊销。|
|挂起|1|待处理的吊销。|
|颁发|2|吊销发出命令。|
|failed|3|吊销失败。|
|吊销|4|吊销。|




