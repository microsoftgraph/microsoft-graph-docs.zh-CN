---
title: win32LobAppReturnCodeType 枚举类型
description: 指示返回代码的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42491bd49759dbb7642fc968cd8957d5a2948305
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412385"
---
# <a name="win32lobappreturncodetype-enum-type"></a>win32LobAppReturnCodeType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示返回代码的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|failed|0|失败。|
|success|1|成功。|
|softReboot|2|软重启是必需的。|
|hardReboot|3|硬重新启动，则需要。|
|重试|4|重试。|




