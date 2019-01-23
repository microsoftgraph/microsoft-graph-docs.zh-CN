---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20eb1053d3dbf6cb657313f0c68f6c6c84804848
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398980"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a>deviceManagementExchangeConnectorType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Exchange 连接器的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|onPremises|0|连接到内部部署 Exchange 环境。|
|承载|1|连接到 O365 多租户 Exchange 环境|
|serviceToService|2|Intune 服务直接连接到 O365 多租户 Exchange 环境|
|专用|3|连接到 O365 专用 Exchange 环境。|




