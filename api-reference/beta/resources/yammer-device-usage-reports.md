---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9d5a7d2ea6cd8e02e26414618b27acf441444cd
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390051"
---
# <a name="yammer-device-usage-reports"></a>Yammer 设备使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 - Yammer使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。

## <a name="reports"></a>报告

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                    |
| :----------------------------------------------------------- | :-------------- | :--------------- | ---------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | Stream           | 获取用户的 Yammer 设备使用情况的详细信息。 |
| [获取分发用户数](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | Stream           | 按设备类型获取用户数。        |
| [获取用户数](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | Stream           | 按设备类型获取每日用户数。  |


