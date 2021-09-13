---
title: 电子邮件应用使用情况报表
description: 电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 8959d65250cd4f0dfac7b71970730bad8e6cfa8c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118622"
---
# <a name="email-app-usage-reports"></a>电子邮件应用使用情况报表

命名空间：microsoft.graph

电子邮件应用使用情况报表可用于了解用于连接到 Exchange Online 的电子邮件应用数。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报告 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getemailappusageuserdetail.md) | Stream      | 获取用户在不同电子邮件应用中执行的活动的详细信息。 |
| [获取应用用户数](../api/reportroot-getemailappusageappsusercounts.md) | Stream      | 获取每个电子邮件应用的唯一用户数。 |
| [获取用户数](../api/reportroot-getemailappusageusercounts.md) | Stream      | 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。 |
| [获取版本用户数](../api/reportroot-getemailappusageversionsusercounts.md) | Stream      | 按 Outlook 桌面版获取唯一用户数。 |

