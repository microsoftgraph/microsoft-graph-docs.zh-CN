---
title: Microsoft 365激活报告
description: 此Microsoft 365激活报告可让你查看至少一台设备上哪些用户Microsoft 365订阅。 这些报告提供了 Microsoft 365 ProPlus、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备激活的细目。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2b736d72fc8f91164b2559d5678f076ece62462a54b671bb74ade50a64fee3db
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251897"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365激活报告

命名空间：microsoft.graph

此Microsoft 365激活报告可让你查看至少一台设备上哪些用户Microsoft 365订阅。 这些报告提供了 Microsoft 365 ProPlus、Project 和 Visio Pro for Office 365 订阅激活的细目，以及跨桌面和设备激活的细目。 此类报表有助于发现可能需要额外支持才能激活 Office 订阅的用户。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)Microsoft Office激活。

## <a name="reports"></a>报表
| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot-getoffice365activationsuserdetail.md) | Stream      | 获取有关已激活此Microsoft 365。 |
| [获取激活数](../api/reportroot-getoffice365activationcounts.md) | Stream      | 获取桌面Microsoft 365激活次数。 |
| [获取用户数](../api/reportroot-getoffice365activationsusercounts.md) | Stream      | 获取在桌面或设备上激活 Office 订阅的已启用用户数。 |

