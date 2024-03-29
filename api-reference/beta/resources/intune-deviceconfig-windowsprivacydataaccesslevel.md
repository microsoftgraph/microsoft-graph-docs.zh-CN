---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定特定用户隐私数据Windows的访问级别。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c45d78e06ac44fc30cb631359f213a90d8ba8f6a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105893"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

确定特定用户隐私数据Windows的访问级别。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未指定访问级别，没有意图。 设备的行为类似于 UserInControl 或 ForceAllow。 它可能取决于已访问的隐私数据、Windows版本和其他因素。|
|forceAllow|1|将允许应用访问指定的隐私数据。|
|forceDeny|2|应用程序将被拒绝访问指定的隐私数据。|
|userInControl|3|当应用尝试访问指定的隐私数据时，将提示用户。|



