---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 55f706fb15ab2c6f40800ea9b2170977de8b3c65
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455742"
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
|autoInstallAndRebootWithoutEndUserControl|5|在没有最终用户控制的情况下自动安装和重启|



