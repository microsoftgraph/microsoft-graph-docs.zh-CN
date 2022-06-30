---
title: 在 Excel 中管理会话和持久性
description: 了解如何以最有效的方式在 Microsoft Graph 中使用 Excel API。 了解调用 API 的三种模式以及相关的请求类型。
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
ms.openlocfilehash: b2b38c20f3ae1613d9330271cd73af56bb7d33c8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440829"
---
# <a name="manage-sessions-and-persistence-in-excel"></a>在 Excel 中管理会话和持久性

如果应用程序需要对 Microsoft Graph 中的 Excel API 进行一两次以上的调用，请创建一个会话，并通过每个请求传递会话 ID。 请求中存在会话 ID 可确保以最有效的方式使用 Excel API。

可通过以下三个模式之一下调用 Excel API：

- **持久会话：** 对工作簿所做的所有更改将保留 (保存到工作簿) 。 这是使用 Excel API 最高效且性能最佳的方式。

- **非持久会话：** API 所做的更改不会保存到源位置。 而是，Excel 后端服务器将保留文件的临时副本，用于反映在特定 API 会话期间所做的更改。 Excel 会话过期时，这些更改将丢失。 此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。

- **无会话：** API 调用不会传递会话 ID。 Excel 服务器必须查找每个操作的工作簿的服务器副本。 这不是调用 Excel API 的有效方式，但它适用于进行某些类型的隔离请求。

若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。

> [!NOTE]
> Excel API 无需使用会话标头。 但是，建议你使用会话标头来提高性能。 如果不使用会话标头，API 调用过程中进行的更改 _仅_ 保持在该文件中。  

## <a name="request-types"></a>请求类型

建议的 Excel API [错误处理](workbook-error-handling.md) 基于请求类型、错误代码和状态代码。 下面是请求类型：

- **CreateSession 请求：** 用于创建持久性会话或非永久性会话。 在成功响应中，会话 ID 将在响应正文中的 **ID** 属性中返回。 有关详细信息，请参阅 [“创建会话](/graph/api/workbook-createsession)”。
- **会话请求：** 遵循 CreateSession 请求的后续请求。 它们通常包含标 `workbook-session-id: {session-id}` 头。 异常是使用长时间运行的操作模式的轮询状态请求。 有关详细信息，请参阅使用 [需要很长时间才能完成的 API](./workbook-best-practice.md#work-with-apis-that-take-a-long-time-to-complete)。
- **无会话请求：** 在无会话模式下使用。 这些请求没有 `workbook-session-id: {session-id}` 标头。  

## <a name="next-steps"></a>后续步骤

要了解如何创建和使用会话，请参阅[创建会话参考主题](/graph/api/workbook-createsession)。

## <a name="see-also"></a>另请参阅

* [使用 Microsoft Graph 编写 Excel 工作簿](excel-write-to-workbook.md)
* [通过 Microsoft Graph 使用 Excel 工作簿函数](excel-use-functions.md)
* [通过 Microsoft Graph 更新 Excel 区域的格式](excel-update-range-format.md)
* [通过 Microsoft Graph 显示 Excel 图表图像](excel-display-chart-image.md)
* [使用 Excel REST API](/graph/api/resources/excel)