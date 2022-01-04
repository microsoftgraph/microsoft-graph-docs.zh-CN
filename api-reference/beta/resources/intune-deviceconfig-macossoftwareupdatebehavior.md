---
title: macOSSoftwareUpdateBehavior 枚举类型
description: macOS 软件更新的更新行为选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a0fa894d17e126287ccb1e1c63e36160cf2dcd3e
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/04/2022
ms.locfileid: "61712080"
---
# <a name="macossoftwareupdatebehavior-enum-type"></a>macOSSoftwareUpdateBehavior 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

macOS 软件更新的更新行为选项。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置。|
|default|1|下载和/或安装软件更新，具体取决于当前设备状态。|
|downloadOnly|2|在不安装的情况下下载软件更新。|
|installASAP|3|安装已下载的软件更新。|
|notifyOnly|4|下载软件更新，然后通过应用商店通知用户。|
|installLater|5|下载软件更新，并稍后安装它。|




