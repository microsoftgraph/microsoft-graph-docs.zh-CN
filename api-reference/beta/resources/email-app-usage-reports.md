---
title: 电子邮件应用使用情况报表
description: 你可以看到有多少电子邮件应用用于连接到Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。
ms.localizationpriority: medium
author: sarahwxy
ms.prod: reports
doc_type: conceptualPageType
ms.openlocfilehash: 341dda4411e39cd028f6f5921e12e1c5b5bd5d7f
ms.sourcegitcommit: 42e0e15ff90815e0126c34b928405486cfb1ed86
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2021
ms.locfileid: "61044804"
---
# <a name="email-app-usage-reports"></a>电子邮件应用使用情况报表

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

你可以看到有多少电子邮件应用用于连接到Exchange Online。 此外，还可以了解使用的 Outlook 应用版本，这有助于跟进应升级到受支持 Outlook 版本的用户。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报告 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。

## <a name="reports"></a>报表

| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取用户详细信息](../api/reportroot-getemailappusageuserdetail.md) | Stream          | Stream           | 获取用户在不同电子邮件应用中执行的活动的详细信息。 |
| [获取应用用户数](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | Stream           | 获取每个电子邮件应用的唯一用户数。                 |
| [获取用户数](../api/reportroot-getemailappusageusercounts.md) | Stream          | Stream           | 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。 |
| [获取版本用户数](../api/reportroot-getemailappusageversionsusercounts.md) | Stream          | Stream           | 按 Outlook 桌面版获取唯一用户数。    |


