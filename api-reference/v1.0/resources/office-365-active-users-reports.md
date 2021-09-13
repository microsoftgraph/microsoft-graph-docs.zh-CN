---
title: Microsoft 365活动用户报告
description: 可以使用活动Microsoft 365报告了解组织中个人使用的产品许可证数量，并向下钻取有关哪些用户使用哪些产品的信息。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: da908b20bf182ac45b5deb29da1c04c0207382fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094217"
---
# <a name="microsoft-365-active-users-reports"></a>Microsoft 365活动用户报告

命名空间：microsoft.graph

可以使用活动Microsoft 365报告了解组织中个人使用的产品许可证数量，并向下钻取有关哪些用户使用哪些产品的信息。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。

> **备注：** 若要了解不同报表视图和名称的详细信息，请参阅 [Microsoft 365 报表 - 活动用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。

## <a name="reports"></a>报表
| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activeuserdetail.md) | Stream      | 获取有关 Microsoft 365 活动用户的详细信息。 |
| [获取用户数](../api/reportroot-getoffice365activeusercounts.md) | Stream      | 按产品获取报表周期内的每日活跃用户数。 |
| [获取服务用户数](../api/reportroot-getoffice365servicesusercounts.md) | Stream      | 按活动类型和服务获取用户数。 |

