---
title: appManagementLevel 枚举类型
description: 应用的管理级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d97b5973842d281dc8631a92c6818cb1d7026ae
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66669019"
---
# <a name="appmanagementlevel-enum-type"></a>appManagementLevel 枚举类型

命名空间：microsoft.graph

> **重要：** /beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产用途。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用的管理级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|未指定|0|Unspecified|
|非 托管|1|非 托管|
|Mdm|2|MDM|
|androidEnterprise|4|Android Enterprise|
|androidEnterpriseDedicatedDevicesWithAzureAdSharedMode|8 |采用 Azure AD 共享模式的 Android Enterprise 专用设备|
|androidOpenSourceProjectUserAssociated|16|Android 开源项目 (AOSP) 设备|
|androidOpenSourceProjectUserless|32|Android 开源项目 (AOSP) 无用户设备|




