---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
author: tfitzmac
ms.openlocfilehash: d1bf3903b71dbd06be9151d67a925f374eb1f803
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344042"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

自动更新模式的的可能值。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|用户定制|0|用户定义，默认值、 没有用途。|
|notifyDownload|1|在下载通知。|
|autoInstallAtMaintenanceTime|2|自动安装在维护时间。|
|autoInstallAndRebootAtMaintenanceTime|3|自动安装和维护时间重新启动。|
|autoInstallAndRebootAtScheduledTime|4|自动安装并在计划时间重新启动。|
|autoInstallAndRebootWithoutEndUserControl|5|自动安装并重新启动不最终用户控件|





