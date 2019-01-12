---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e9e50a4475ca2d57b3f38567703046588d4fb3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986430"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a>deviceManagementExchangeConnectorType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Exchange 连接器的类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|onPremises|0|连接到内部部署 Exchange 环境。|
|承载|1|连接到 O365 多租户 Exchange 环境|
|serviceToService|2|Intune 服务直接连接到 O365 多租户 Exchange 环境|
|专用|3|连接到 O365 专用 Exchange 环境。|



