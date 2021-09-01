---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: 连接器的当前Exchange状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1d8ad720b4b03fb157b71506b055bab9916443b4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58801057"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a>deviceManagementExchangeConnectorStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

连接器的当前Exchange状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|不存在连接器。|
|connectionPending|1|挂起到 Exchange 的连接。|
|connected|2|连接到Exchange环境|
|已断开连接|3|与 Exchange 环境断开连接|



