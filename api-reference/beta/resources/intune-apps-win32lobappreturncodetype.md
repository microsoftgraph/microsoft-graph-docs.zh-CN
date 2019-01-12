---
title: win32LobAppReturnCodeType 枚举类型
description: 指示返回代码的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad1fc25c3194d7bb6e930fa81660fcc4b882f0ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990129"
---
# <a name="win32lobappreturncodetype-enum-type"></a>win32LobAppReturnCodeType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

指示返回代码的类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|failed|0|失败。|
|success|1|成功。|
|softReboot|2|软重启是必需的。|
|hardReboot|3|硬重新启动，则需要。|
|重试|4|重试。|





