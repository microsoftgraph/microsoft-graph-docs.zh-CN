---
title: Excel 工作簿和图表 API 概述
description: Excel 是一个提高工作效率不可或缺的工具。 所有行业和工作职能的用户都将其视为用于存储、跟踪和操作各类数据的工具。 从简单的任务跟踪和数据管理，到复杂的计算和专业报告，Excel 可用于处理各种各样的任务。 你可以使用 Microsoft Graph 中的 Excel REST API 扩展数据、计算、报告和仪表板的价值。
ms.localizationpriority: high
author: lumine2008
ms.prod: excel
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1380539804bdd4859385cc887a691b89b3e82965
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136108"
---
# <a name="excel-workbooks-and-charts-api-overview"></a>Excel 工作簿和图表 API 概述

Excel 是一个提高工作效率不可或缺的工具。 所有行业和工作职能的用户都将其视为用于存储、跟踪和操作各类数据的工具。 从简单的任务跟踪和数据管理，到复杂的计算和专业报告，Excel 可用于处理各种各样的任务。 你可以使用 Microsoft Graph 中的 Excel REST API 扩展数据、计算、报告和仪表板的价值。

> [!VIDEO https://www.youtube-nocookie.com/embed/I1rSkJww2Dk]

## <a name="why-integrate-with-excel"></a>为什么与 Excel 集成？

你可以使用 Microsoft Graph 来让 Web 和移动应用程序读取和修改存储在 OneDrive、SharePoint 或其他支持的存储平台中的 Excel 工作簿。

### <a name="perform-calculations"></a>执行计算

用户喜欢他们可以轻松地在 Excel 中执行深入而复杂的计算。 现在，你可以使用 Excel 强大的计算引擎，并且可以立即得到结果。 例如，按揭贷款计算器通过简单的 API 调用（包括付款的本金、利率和付款次数）即可利用 Excel 中的 PMT 函数。 Excel 将进行所有的复杂计算，并立即返回每月付款。 当前提供有 300 多个 Excel 工作表函数，你可以完全访问 Excel 目前支持的各种公式。 不需要反复重建复杂业务模型。 开发者可以对 Excel 编程以立即执行这些计算，并使用简单 API 调用检索这些结果。

### <a name="generate-reports-and-analyze-results"></a>生成报告并分析结果

Excel 是一款灵活的报告和分析工具，范围从简单的数据表到复杂的专业仪表板。 现在，我们为你提供了访问 Excel 报告功能的完整权限，使 Excel 成为 Microsoft 365 中的一个在线报告服务。 想象一下：用户目前创建和依赖的所有报告方案都拉入到一个自定义应用，以创建专业图表或智能分析大量数据，从而将 Excel 无缝融合到这些自定义的体验中。

### <a name="store-and-track-data"></a>存储和跟踪数据

Excel 还是一款出色的存储和跟踪数据的工具。 如果信息存储在工作簿中，则与 Microsoft 365 集成的任何应用都可以访问该数据。 可以从自定义解决方案读取其内容，并且这些解决方案可以使用 Excel 来存储数据。

>**注意：** Excel REST API 仅支持 Office Open XML 文件格式的工作簿（扩展名为 `.xlsx` 的文件）。 不支持扩展名为 `.xls` 的工作簿。 

### <a name="using-the-excel-rest-api"></a>使用 Excel REST API
可以使用 Microsoft Graph，使 Web 和移动应用程序可以读取和修改存储在 OneDrive、SharePoint 或其他支持的存储平台中的 Excel 工作簿。`Workbook`（或 Excel 文件）资源通过关系包含所有其他 Excel 资源。可以通过识别文件在该 URL 中的位置，借助 驱动器 API 访问工作簿。例如：

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`

`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`

可以通过使用标准 REST API 访问一组 Excel 对象（例如表、区域或图表），以便对工作簿执行创建、读取、更新和删除 (CRUD) 操作。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 Excel API](/graph/api/resources/excel?view=graph-rest-1.0)
- [Microsoft Graph beta 中的 Excel API](/graph/api/resources/excel?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

* [通过 Microsoft Graph 管理 Excel 会话](excel-manage-sessions.md)
* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [通过 Microsoft Graph 显示 Excel 图表图像](excel-display-chart-image.md)
* [使用 Excel REST API](/graph/api/resources/excel?view=graph-rest-1.0)
