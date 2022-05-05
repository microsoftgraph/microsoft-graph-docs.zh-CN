---
title: resultantAppState 枚举类型
description: 单个设备上应用程序状态的可能状态列表。 当设备联系Intune服务并找到有针对性的应用程序强制实施意向时，将记录执行状态，并在图形 API中访问。 由于应用程序状态是在设备与Intune服务交互期间标识的，因此状态记录不会在应用程序组分配时立即显示;它仅在服务中评估分配后创建，并且设备在签入期间开始接收策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5d05a7ac37c525e5a598e158a386dd1d14c35a23
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211920"
---
# <a name="resultantappstate-enum-type"></a>resultantAppState 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

单个设备上应用程序状态的可能状态列表。 当设备联系Intune服务并找到有针对性的应用程序强制实施意向时，将记录执行状态，并在图形 API中访问。 由于应用程序状态是在设备与Intune服务交互期间标识的，因此状态记录不会在应用程序组分配时立即显示;它仅在服务中评估分配后创建，并且设备在签入期间开始接收策略。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|安装|1|应用程序安装时不会出错。|
|失败|2|应用程序安装失败。|
|notInstalled|3|未安装应用程序。|
|uninstallFailed|4|应用程序无法卸载。|
|pendingInstall|5|正在安装应用程序。|
|unknown|99|应用程序的状态未知。|
|notApplicable|-1|应用程序不适用。|




