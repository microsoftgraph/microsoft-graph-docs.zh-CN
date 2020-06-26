---
title: Microsoft 365 激活报告
description: Microsoft 365 激活报告可让你查看在至少一个设备上已激活其 Microsoft 365 订阅的用户。 这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备的激活细目。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 34bebb8edb7d83ca631d93add90a7e2810849c3d
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898168"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365 激活报告

命名空间：microsoft.graph

Microsoft 365 激活报告可让你查看在至少一个设备上已激活其 Microsoft 365 订阅的用户。 这些报告提供了 Microsoft 365 专业增强版、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备的激活细目。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅[microsoft 365 报表-Microsoft Office 激活](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)。

## <a name="reports"></a>报表
| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | 获取已激活 Microsoft 365 的用户的详细信息。 |
| [获取激活数](../api/reportroot-getoffice365activationcounts.md) | Stream      | 获取桌面和设备上的 Microsoft 365 激活次数。 |
| [获取用户数](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | 获取在桌面或设备上激活 Office 订阅的已启用用户数。 |
