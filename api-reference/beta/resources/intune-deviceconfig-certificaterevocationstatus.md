---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1c77e267da5528088a7a8ef6400a872790aaf3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983119"
---
# <a name="certificaterevocationstatus-enum-type"></a>certificateRevocationStatus 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

证书吊销状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未被吊销。|
|挂起|1|待处理的吊销。|
|颁发|2|吊销发出命令。|
|failed|3|吊销失败。|
|吊销|4|吊销。|





