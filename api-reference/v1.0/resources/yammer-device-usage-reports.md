---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f4736d92a990c94d2017cc8a26396a3cc4f6e04f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897748"
---
# <a name="yammer-device-usage-reports"></a>Yammer 设备使用情况报表

命名空间：microsoft.graph

Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[Microsoft 365 报表-Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream      | 获取用户的 Yammer 设备使用情况的详细信息。 |
| [获取分发用户数](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream      | 按设备类型获取用户数。  |
| [获取用户数](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream      | 按设备类型获取每日用户数。 |
