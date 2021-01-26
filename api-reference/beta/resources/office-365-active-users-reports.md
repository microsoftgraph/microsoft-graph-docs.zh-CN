---
title: Microsoft 365 活动用户报告
description: 可以使用 Microsoft 365 活动用户报告了解组织中个人使用的产品许可证数量，并深入了解哪些用户使用哪些产品。 此报表可帮助管理员确定未被充分利用的产品或是可能需要其他培训或信息的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ee227bf0413944bdd648de64f32bf4f6ab9f3d70
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980768"
---
# <a name="microsoft-365-active-users-reports"></a>Microsoft 365 活动用户报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

可以使用 Microsoft 365 活动用户报告了解组织中个人使用的产品许可证数量，并深入了解哪些用户使用哪些产品。 此报表可帮助管理员确定未被充分利用的产品或是可能需要其他培训或信息的用户。

> **备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。

## <a name="reports"></a>报告
| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | 获取有关 Microsoft 365 活动用户的详细信息。 |
| [获取用户计数](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | 按产品获取报表周期内的每日活跃用户数。 |
| [获取服务用户数](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | 按活动类型和服务获取用户数。 |


