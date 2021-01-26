---
title: Microsoft 365 激活报告
description: Microsoft 365 激活报告可让你查看哪些用户在至少一台设备上激活了 Microsoft 365 订阅。 这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备激活的细分。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 30d9fa1799367e0589115c56dd069db6ca7b1ff9
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981044"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365 激活报告

命名空间：microsoft.graph

Microsoft 365 激活报告可让你查看哪些用户在至少一台设备上激活了 Microsoft 365 订阅。 这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备激活的细分。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 -](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)Microsoft Office激活。

## <a name="reports"></a>报告
| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | 获取有关已激活 Microsoft 365 的用户的详细信息。 |
| [获取激活数](../api/reportroot-getoffice365activationcounts.md) | Stream      | 获取桌面和设备上 Microsoft 365 激活的计数。 |
| [获取用户计数](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | 获取在桌面或设备上激活 Office 订阅的已启用用户数。 |

