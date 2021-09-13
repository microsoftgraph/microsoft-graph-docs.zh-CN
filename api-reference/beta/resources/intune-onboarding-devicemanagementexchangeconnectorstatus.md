---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: 连接器的当前Exchange状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: db5845b0208bf528dc20a30b750bc6bb64e6e387
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080896"
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



