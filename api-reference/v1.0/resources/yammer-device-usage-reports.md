---
title: Yammer 设备使用情况报表
description: Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7b5be6f8c5594239aac6a7154b66e08fe04a6a10
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139329"
---
# <a name="yammer-device-usage-reports"></a>Yammer 设备使用情况报表

命名空间：microsoft.graph

Yammer 设备使用情况报表可用于了解用户使用什么设备在 Yammer 上进行交互。 可以按设备类型查看在一段选定时间内的用户数，并按用户查看详细信息。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)Yammer使用情况。

## <a name="reports"></a>报告

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream      | 获取用户的 Yammer 设备使用情况的详细信息。 |
| [获取分发用户数](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream      | 按设备类型获取用户数。  |
| [获取用户数](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream      | 按设备类型获取每日用户数。 |

