---
title: Office 365 活跃用户报表
description: 您可以使用 Office 365 活动用户报告以找出多少个产品许可证正在使用的组织中的个人和向下钻取有关哪些用户正在使用哪些产品的信息。 此报告可帮助管理员识别未充分利用的产品或可能需要其他培训或信息的用户。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 958cf769a2b54f1d22cdc315ee250cb1e677c301
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970505"
---
# <a name="office-365-active-users-reports"></a>Office 365 活跃用户报表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以使用 Office 365 活动用户报告以找出多少个产品许可证正在使用的组织中的个人和向下钻取有关哪些用户正在使用哪些产品的信息。 此报告可帮助管理员识别未充分利用的产品或可能需要其他培训或信息的用户。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。

## <a name="reports"></a>报表
| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | 获取 Office 365 活跃用户的详细信息。 |
| [获取用户数](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | 按产品获取报表周期内的每日活跃用户数。 |
| [获取服务用户数](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | 按活动类型和服务获取用户数。 |
