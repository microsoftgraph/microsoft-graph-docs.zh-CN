---
title: macOSGatekeeperAppSources 枚举类型
description: macOS 网关守卫的应用源选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1fdf2aa4009c9dedb49d046e7f912c0d23cc85eee92f784fa19f7398b725bc2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141978"
---
# <a name="macosgatekeeperappsources-enum-type"></a>macOSGatekeeperAppSources 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

macOS 网关守卫的应用源选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，无意图。|
|macAppStore|1 |只能运行来自 Mac AppStore 的应用程序。|
|macAppStoreAndIdentifiedDevelopers|2 |只有来自 Mac AppStore 和识别的开发人员的应用才能运行。|
|任意位置|3 |可以运行来自任何位置的应用。|




