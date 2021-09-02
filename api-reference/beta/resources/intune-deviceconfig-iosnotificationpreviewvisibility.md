---
title: iosNotificationPreviewVisibility 枚举类型
description: 确定通知预览何时在 iOS 设备上可见。 预览可以包含邮件和邮件 (中的文本) 以及日历 (邀请详细信息) 。 配置后，它将覆盖用户定义的预览设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a3f7426134ecf4a5fec3f71cdc33654df292b30
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58759664"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a>iosNotificationPreviewVisibility 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定通知预览何时在 iOS 设备上可见。 预览可以包含邮件和邮件 (中的文本) 以及日历 (邀请详细信息) 。 配置后，它将覆盖用户定义的预览设置。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|不会覆盖通知预览设置。|
|alwaysShow|1|始终显示通知预览。|
|hideWhenLocked|2|仅在设备解锁时显示通知预览。|
|neverShow|3|从不显示通知预览。|



