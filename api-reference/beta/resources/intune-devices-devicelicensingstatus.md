---
title: deviceLicensingStatus 枚举类型
description: 指示启用基于 Windows 设备的订阅后的设备许可状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c0ff1ff53acd502fc6c92923b0a80a99e039d280
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671677"
---
# <a name="devicelicensingstatus-enum-type"></a>deviceLicensingStatus 枚举类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示启用基于 Windows 设备的订阅后的设备许可状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|licenseRefreshStarted|0|启动许可证刷新时将设置此状态。|
|licenseRefreshPending|1|当许可证刷新挂起时，将设置此状态。|
|deviceIsNotAzureActiveDirectoryJoined|2|如果设备未加入 Azure Active Directory，则会设置此状态。|
|verifyingMicrosoftDeviceIdentity|3|验证 Microsoft 设备标识时，将设置此状态。|
|deviceIdentityVerificationFailed|4|当 Microsoft 设备标识验证失败时，将设置此状态。|
|verifyingMirosoftAccountIdentity|5|验证 Microsoft 帐户标识时，将设置此状态。|
|mirosoftAccountVerificationFailed|6 |当 Microsoft 帐户标识验证失败时，将设置此状态。|
|acquiringDeviceLicense|7 |获取设备许可证时将设置此状态。|
|refreshingDeviceLicense|8 |刷新设备许可证时将设置此状态。|
|deviceLicenseRefreshSucceed|9 |当设备许可证刷新成功时，将设置此状态。|
|deviceLicenseRefreshFailed|10|当设备许可证刷新失败时，将设置此状态。|
|removingDeviceLicense|11|删除设备许可证时，将设置此状态。|
|deviceLicenseRemoveSucceed|12 |当设备许可证删除成功时，将设置此状态。|
|deviceLicenseRemoveFailed|13|当设备许可证删除失败时，将设置此状态。|
|unknownFutureValue|14|此处作为将来扩展的占位符放置在此处。|
|unknown|-1|默认值。 在无法确定状态时设置为未知。|




