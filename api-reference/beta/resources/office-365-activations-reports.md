---
title: Office 365 激活报表
description: Office 365 激活报告提供的用户已激活其至少一个设备上的 Office 365 订阅的视图。 它提供了 Office 365 ProPlus、 Project 和 Visio Pro for Office 365 订阅激活的细分以及激活的细分结构跨桌面和设备。 此报告可帮助您识别可能需要其他支持激活其 Office 订阅的用户。
localization_priority: Normal
ms.openlocfilehash: 2576579879e60573a9ed70f805fe07532bab8ad8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822216"
---
# <a name="office-365-activations-reports"></a>Office 365 激活报表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

Office 365 激活报告提供的用户已激活其至少一个设备上的 Office 365 订阅的视图。 它提供了 Office 365 ProPlus、 Project 和 Visio Pro for Office 365 订阅激活的细分以及激活的细分结构跨桌面和设备。 此报告可帮助您识别可能需要其他支持激活其 Office 订阅的用户。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。

## <a name="reports"></a>报表
| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | 获取已激活 Office 365 的用户的详细信息。 |
| [获取激活数](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | 获取桌面和设备上激活的 Office 365 订阅数。 |
| [获取用户数](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | 获取在桌面或设备上激活 Office 订阅的已启用用户数。 |
