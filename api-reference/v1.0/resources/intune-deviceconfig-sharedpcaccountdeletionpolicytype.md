---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 在共享电脑上删除帐户时的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f41cfc20132577d11d94cdd66d28cdccfa203b4f
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457300"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a>sharedPCAccountDeletionPolicyType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在共享电脑上删除帐户时的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|immediate|0|立即删除。|
|diskSpaceThreshold|1|达到磁盘空间阈值时删除。|
|diskSpaceThresholdOrInactiveThreshold|2|达到磁盘空间阈值或非活动阈值时删除。|



