---
title: Office 365 激活报表
description: Office 365 激活报告为您提供了一个用户在至少一个设备上激活其 Office 365 订阅的视图。 它提供了 office 365 专业增强版、Project 和 Visio Pro for office 365 订阅激活的细目, 以及跨桌面和设备的激活细目。 此报告可帮助您确定可能需要其他支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a0baa50cee545dbbf6f3074e89eafdd91c511ac9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342056"
---
# <a name="office-365-activations-reports"></a>Office 365 激活报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Office 365 激活报告为您提供了一个用户在至少一个设备上激活其 Office 365 订阅的视图。 它提供了 office 365 专业增强版、Project 和 Visio Pro for office 365 订阅激活的细目, 以及跨桌面和设备的激活细目。 此报告可帮助您确定可能需要其他支持才能激活 Office 订阅的用户。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。

## <a name="reports"></a>报表
| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | 获取已激活 Office 365 的用户的详细信息。 |
| [获取激活数](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | 获取桌面和设备上激活的 Office 365 订阅数。 |
| [获取用户数](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | 获取在桌面或设备上激活 Office 订阅的已启用用户数。 |
