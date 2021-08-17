---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ab80ab2f3e811435107fbbc8e1395b16f5c5340c39b4b68a138316d91ecc30b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131190"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自动更新模式的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意图。|
|notifyDownload|1 |下载时通知。|
|autoInstallAtMaintenanceTime|2 |在维护时自动安装。|
|autoInstallAndRebootAtMaintenanceTime|3 |在维护时自动安装和重启。|
|autoInstallAndRebootAtScheduledTime|4 |按计划时间自动安装和重启。|
|autoInstallAndRebootWithoutEndUserControl|5 |在没有最终用户控制的情况下自动安装和重启|
|windowsDefault|6 |重置为Windows默认值。|




