---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f00ce8c6926c953a95081a864d1fb3a0cdfd1bc7
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802500"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a>sharedPCAccountDeletionPolicyType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在共享电脑上删除帐户时的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|immediate|0|立即删除。|
|diskSpaceThreshold|1|达到磁盘空间阈值时删除。|
|diskSpaceThresholdOrInactiveThreshold|2|达到磁盘空间阈值或非活动阈值时删除。|



