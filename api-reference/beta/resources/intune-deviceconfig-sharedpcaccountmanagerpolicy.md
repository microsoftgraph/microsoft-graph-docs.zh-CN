---
title: sharedPCAccountManagerPolicy 资源类型
description: 共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e5803a3600bc4ce0f8366cfceba1813e23dbab3f2e950bd8cd39cc15cb9df61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226362"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>sharedPCAccountManagerPolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




