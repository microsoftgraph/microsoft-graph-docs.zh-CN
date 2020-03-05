---
title: macOSGatekeeperAppSources 枚举类型
description: MacOS 网关的应用程序源选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7e0990d063d2f50045b3d5de7f4cce4f9f32943b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526109"
---
# <a name="macosgatekeeperappsources-enum-type"></a>macOSGatekeeperAppSources 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

MacOS 网关的应用程序源选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|设备默认值，无意向。|
|macAppStore|1 |只有 Mac AppStore 中的应用可以运行。|
|macAppStoreAndIdentifiedDevelopers|2 |只有 Mac AppStore 和已确定的开发人员的应用可以运行。|
|无论|3 |可以从任意位置运行应用程序。|



