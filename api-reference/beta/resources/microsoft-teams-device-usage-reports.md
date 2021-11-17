---
title: Microsoft Teams 设备使用情况报告
description: '使用 Microsoft Teams设备使用情况报告，深入了解Microsoft Teams设备使用情况。 '
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ff56158cb30f069a19c0fb5e67c49df157709b81
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044797"
---
# <a name="microsoft-teams-device-usage-reports"></a>Microsoft Teams 设备使用情况报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft Teams设备使用情况报告，深入了解Microsoft Teams设备使用情况。 

## <a name="methods"></a>方法

| 方法                                                       | 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getteamsdeviceusageuserdetail.md) | Stream      | 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。      |
| [获取用户数](../api/reportroot-getteamsdeviceusageusercounts.md) | Stream      | 按设备类型获取许可Microsoft Teams每天的唯一用户数。 |
| [获取用户总数](../api/reportroot-getteamsdeviceusagetotalusercounts.md) | Stream      | 按设备类型获取Microsoft Teams用户或非许可用户的每日唯一数量。 |
| [获取分发用户数](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | Stream      | 按设备类型Microsoft Teams许可证用户数。 |
| [获取分发用户总数](../api/reportroot-getteamsdeviceusagedistributiontotalusercounts.md) | Stream      | 按设备类型Microsoft Teams获取许可用户或非许可用户的唯一用户数。 |


