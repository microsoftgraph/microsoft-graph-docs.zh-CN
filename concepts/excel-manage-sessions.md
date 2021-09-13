---
title: 通过 Microsoft Graph 管理 Excel 会话和暂留
description: 如果应用程序需要对 Excel API 进行多次（或两次以上）的调用，则应创建一个会话并为每个请求传递会话 ID。 请求中的会话 ID 可确保你以最有效的方式使用 Excel API。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: fc3639b76fbfca470a1b6a4d9e51b4ad783eccc2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136073"
---
# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a>通过 Microsoft Graph 管理 Excel 会话和暂留

如果应用程序需要对 Excel API 进行多次（或两次以上）的调用，则应创建一个会话并为每个请求传递会话 ID。 请求中的会话 ID 可确保你以最有效的方式使用 Excel API。

可通过以下三个模式之一下调用 Excel API：

1. **永久会话** - 对工作簿所做的全部更改保持（保存）到工作簿。 这是使用 Excel API 最高效且性能最佳的方式。
2. **非永久会话** - 不会将 API 所做的更改保存到源位置。 而是，Excel 后端服务器将保留文件的临时副本，用于反映在特定 API 会话期间所做的更改。 Excel 会话过期时，这些更改将丢失。 此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。
3. **无会话** - API 调用不传递会话 ID。Excel 服务器必须为每个操作找到服务器的工作簿副本。 这不是调用 Excel API 的有效方式，但它适用于进行某些类型的隔离请求。

若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。

>**注意：** Excel API 不需要会话标头也能起作用。但是，建议你使用会话标头来提高性能。如果不使用会话标头，API 调用过程中进行的更改 _仅_ 保持在该文件中。  

## <a name="request-types"></a>请求类型
针对[API 的建议](workbook-error-handling.md)错误Excel基于请求类型、错误代码和状态代码。 请求类型如下：

- **CreateSession 请求** - 用于创建永久会话或非永久会话。 在成功响应中，会话 ID 将在响应正文的 **id** 属性中返回。 有关详细信息，请参阅创建 [会话](/graph/api/workbook-createsession?view=graph-rest-1.0)。
- **会话请求** - CreateSession 请求后的后续请求。 它们通常包括 `workbook-session-id: {session-id}` 标头。 例外情况是轮询状态请求，它使用长时间运行的操作模式。 有关详细信息，[请参阅使用需要很长时间才能完成的 API。](./workbook-best-practice.md#working-with-apis-that-take-a-long-time-to-complete)
- **无会话请求** - 在无会话模式下使用。 这些请求没有 `workbook-session-id: {session-id}` 标头。  

## <a name="next-steps"></a>后续步骤
要了解如何创建和使用会话，请参阅[创建会话参考主题](/graph/api/workbook-createsession?view=graph-rest-1.0)。

## <a name="see-also"></a>另请参阅
* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [通过 Microsoft Graph 显示 Excel 图表图像](excel-display-chart-image.md)
* [使用 Excel REST API](/graph/api/resources/excel?view=graph-rest-1.0)
