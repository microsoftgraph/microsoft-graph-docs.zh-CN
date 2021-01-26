---
title: Microsoft 365 活动用户报告
description: 可以使用 Microsoft 365 活动用户报告来了解组织中个人使用的产品许可证数量，并深入了解哪些用户正在使用哪些产品。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e795b58eaae7ecd428f1473b277cd6bc65cbf09d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981023"
---
# <a name="microsoft-365-active-users-reports"></a>Microsoft 365 活动用户报告

命名空间：microsoft.graph

可以使用 Microsoft 365 活动用户报告来了解组织中个人使用的产品许可证数量，并深入了解哪些用户正在使用哪些产品。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。

> **备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。

## <a name="reports"></a>报告
| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activeuserdetail.md) | Stream      | 获取有关 Microsoft 365 活动用户的详细信息。 |
| [获取用户计数](../api/reportroot-getoffice365activeusercounts.md) | Stream      | 按产品获取报表周期内的每日活跃用户数。 |
| [获取服务用户数](../api/reportroot-getoffice365servicesusercounts.md) | Stream      | 按活动类型和服务获取用户数。 |

