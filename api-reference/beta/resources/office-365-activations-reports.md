---
title: Microsoft 365激活报告
description: 此Microsoft 365激活报告可让你查看至少一个设备上Microsoft 365激活其订阅的用户。 它提供了 Microsoft 365 ProPlus、Project 和 Visio Pro for Microsoft 365 订阅激活的细目，以及跨桌面和设备激活的细目。 此报告可帮助你识别可能需要额外支持才能激活其订阅Office用户。
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: ca3a0218b288105982cb67664629a467a67d596a
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390625"
---
# <a name="microsoft-365-activations-reports"></a>Microsoft 365激活报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此Microsoft 365激活报告可让你查看至少一个设备上Microsoft 365激活其订阅的用户。 它提供了 Microsoft 365 ProPlus、Project 和 Visio Pro for Microsoft 365 订阅激活的细目，以及跨桌面和设备激活的细目。 此报告可帮助你识别可能需要额外支持才能激活其订阅Office用户。

> **注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 - Microsoft Office激活。](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60)

## <a name="reports"></a>报告
| 函数                                                     | CSV 返回类型 | JSON 返回类型 | 说明                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [获取用户详细信息](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | Stream           | 获取有关已激活用户Microsoft 365。    |
| [获取激活数](../api/reportroot-getoffice365activationcounts.md) | Stream          | Stream           | 获取桌面Microsoft 365激活次数。 |
| [获取用户数](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | Stream           | 获取在桌面或设备上激活 Office 订阅的已启用用户数。 |


