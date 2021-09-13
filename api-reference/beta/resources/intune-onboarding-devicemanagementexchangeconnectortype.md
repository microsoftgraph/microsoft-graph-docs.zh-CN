---
title: deviceManagementExchangeConnectorType 枚举类型
description: 连接器Exchange类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0c334ea576a92e8d42084a2c31dc32393dd29606
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080868"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a>deviceManagementExchangeConnectorType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

连接器Exchange类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|onPremises|0|连接到本地部署Exchange环境。|
|托管|1|连接到 O365 多租户Exchange环境|
|serviceToService|2|Intune 服务直接连接到 O365 多租户Exchange环境|
|dedicated|3|连接到 O365 专用Exchange环境。|



