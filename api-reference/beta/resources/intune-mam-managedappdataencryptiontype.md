---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
author: tfitzmac
ms.openlocfilehash: 6bd23f6cd590724c2c981ddf2c3087ead4c21817
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326115"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表向其应用程序数据进行加密托管应用程序的级别
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据进行加密根据设备上的默认设置。|
|afterDeviceRestart|1|应用程序数据进行加密时重新启动设备。|
|whenDeviceLockedExceptOpenFiles|2|与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据|
|whenDeviceLocked|3|与此策略关联的应用程序数据进行加密时设备锁定|





