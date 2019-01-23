---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d6b7e0ab86af78380f85da8ec37c643e662838c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410992"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>sharedPCAccountManagerPolicy 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accountDeletionPolicy|[sharedPCAccountDeletionPolicyType](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|配置何时删除帐户。 可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。|
|cacheAccountsAboveDiskFreePercentage|Int32|设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。 仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。 有效值为 0 至 100|
|inactiveThresholdDays|Int32|指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。 仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。|
|removeAccountsBelowDiskFreePercentage|Int32|设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。 将首先删除处于非活动状态时间最长的帐户。 仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。 有效值为 0 至 100|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```




