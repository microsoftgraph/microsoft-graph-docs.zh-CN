---
title: win32LobAppRegistryDetectionType 枚举类型
description: 包含所有支持的注册表数据检测类型。
author: tfitzmac
ms.openlocfilehash: d47d13c01d282d73d65f559e016bde5f74248158
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362487"
---
# <a name="win32lobappregistrydetectiontype-enum-type"></a>win32LobAppRegistryDetectionType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含所有支持的注册表数据检测类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置。|
|存在|1|指定的注册表项或值存在。|
|doesNotExist|2|指定的注册表项的值不存在。|
|string|3|字符串值类型。|
|integer|4|整数值类型。|
|version|5|版本值类型。|





