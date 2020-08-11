---
title: Microsoft 365 应用程序使用率报告
description: 使用 Microsoft 365 应用使用情况报告可深入了解组织中的 Microsoft 365 应用程序的使用情况。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f9b83608f3a5859e696c4ea2c52e22e35d291fce
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630400"
---
# <a name="microsoft-365-apps-usage-reports"></a>Microsoft 365 应用程序使用率报告

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 Microsoft 365 应用使用情况报告可深入了解组织中的 Microsoft 365 应用程序的使用情况。

## <a name="methods"></a>方法

| 方法                                                                        | 返回类型                                    | 说明                                                |
| :---------------------------------------------------------------------------- | :--------------------------------------------- | :--------------------------------------------------------- |
| [获取用户详细信息](../api/reportroot-getm365appuserdetail.md)                  | [报告](../resources/intune-shared-report.md) | 获取有关用户使用 Microsoft 365 应用程序的详细信息。 |
| [获取用户数](../api/reportroot-getm365appusercounts.md)                  | [报告](../resources/intune-shared-report.md) | 按应用获取每日唯一用户数。               |
| [获取平台用户计数](../api/reportroot-getm365appplatformusercounts.md) | [报告](../resources/intune-shared-report.md) | 按平台获取每日唯一用户数。          |
