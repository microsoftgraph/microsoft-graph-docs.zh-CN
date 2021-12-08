---
title: androidDeviceOwnerCrossProfileDataSharing 枚举类型
description: 表示跨配置文件数据共享的可能值的枚举。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e30b55d7e99e3d33914b666a2088ad29178890a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348375"
---
# <a name="androiddeviceownercrossprofiledatasharing-enum-type"></a>androidDeviceOwnerCrossProfileDataSharing 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示跨配置文件数据共享的可能值的枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置;此值默认为 CROSS_PROFILE_DATA_SHARING_UNSPECIFIED。|
|crossProfileDataSharingBlocked|1|数据不能从要工作配置文件的个人配置文件和工作配置文件共享到个人配置文件。|
|dataSharingFromWorkToPersonalBlocked|2|阻止用户将工作配置文件的数据共享到个人配置文件中的应用。 个人数据可以与工作应用共享。|
|crossProfileDataSharingAllowed|3|两个配置文件的数据都可以与其他配置文件共享。|
|unkownFutureValue|4|保留的 (未知未来值，当前未) |




