---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e3a076fcc88cb64ddeebddcb7f97c3e77c2b34ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136479"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自动更新模式的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|notifyDownload|1|下载时通知。|
|autoInstallAtMaintenanceTime|2|在维护时自动安装。|
|autoInstallAndRebootAtMaintenanceTime|3|在维护时自动安装和重启。|
|autoInstallAndRebootAtScheduledTime|4 |按计划时间自动安装和重启。|
|autoInstallAndRebootWithoutEndUserControl|5 |在没有最终用户控制的情况下自动安装和重启|




