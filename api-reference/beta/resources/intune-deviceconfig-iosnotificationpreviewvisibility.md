---
title: iosNotificationPreviewVisibility 枚举类型
description: 确定何时在 iOS 设备上显示通知预览。 预览可以包括文本 (来自) 日历) 中的邮件和邮件和邀请详细 (信息等内容。 配置后，它将覆盖用户定义的预览设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 607e771ce83858cd22892efa9a377b7997142a24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301601"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a>iosNotificationPreviewVisibility 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定何时在 iOS 设备上显示通知预览。 预览可以包括文本 (来自) 日历) 中的邮件和邮件和邀请详细 (信息等内容。 配置后，它将覆盖用户定义的预览设置。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|通知预览设置不会被覆盖。|
|alwaysShow|1|始终显示通知预览。|
|hideWhenLocked|双面|设备处于解锁状态时仅显示通知预览。|
|neverShow|第三章|从不显示通知预览。|




