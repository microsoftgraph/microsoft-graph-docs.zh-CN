---
title: 通过 Microsoft Graph 管理 Excel 会话和暂留
description: 如果应用程序需要对 Excel API 进行多次（或两次以上）的调用，则应创建一个会话并为每个请求传递会话 ID。 请求中的会话 ID 可确保你以最有效的方式使用 Excel API。
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 151119a2a2861b64db126c8f49d0b916a6f563e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921687"
---
# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a><span data-ttu-id="04074-104">通过 Microsoft Graph 管理 Excel 会话和暂留</span><span class="sxs-lookup"><span data-stu-id="04074-104">Manage sessions and persistence in Excel with Microsoft Graph</span></span>

<span data-ttu-id="04074-105">如果应用程序需要对 Excel API 进行多次（或两次以上）的调用，则应创建一个会话并为每个请求传递会话 ID。</span><span class="sxs-lookup"><span data-stu-id="04074-105">If your application needs to make more than one or two calls to the Excel API, you should create a session and pass the session Id with each request.</span></span> <span data-ttu-id="04074-106">请求中的会话 ID 可确保你以最有效的方式使用 Excel API。</span><span class="sxs-lookup"><span data-stu-id="04074-106">The presence of a session Id in the requests ensures that you are using the Excel API in the most efficient way possible.</span></span>

<span data-ttu-id="04074-107">可通过以下三个模式之一下调用 Excel API：</span><span class="sxs-lookup"><span data-stu-id="04074-107">Excel APIs are called in one of three modes:</span></span>

1. <span data-ttu-id="04074-108">**永久会话** - 对工作簿所做的全部更改保持（保存）到工作簿。</span><span class="sxs-lookup"><span data-stu-id="04074-108">**Persistent session**  All changes made to the workbook are persisted (saved) to the workbook.</span></span> <span data-ttu-id="04074-109">这是使用 Excel API 最高效且性能最佳的方式。</span><span class="sxs-lookup"><span data-stu-id="04074-109">This is the most efficient and best-performing way to use the Excel API.</span></span>
2. <span data-ttu-id="04074-110">**非永久会话** - 不会将 API 所做的更改保存到源位置。</span><span class="sxs-lookup"><span data-stu-id="04074-110">**Non-persistent session**  Changes made by the API are not saved to the source location.</span></span> <span data-ttu-id="04074-111">而是，Excel 后端服务器将保留文件的临时副本，用于反映在特定 API 会话期间所做的更改。</span><span class="sxs-lookup"><span data-stu-id="04074-111">Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session.</span></span> <span data-ttu-id="04074-112">Excel 会话过期时，这些更改将丢失。</span><span class="sxs-lookup"><span data-stu-id="04074-112">When the Excel session expires, the changes are lost.</span></span> <span data-ttu-id="04074-113">此模式可用于需要进行分析或获得计算结果或图表图像的应用，但不会影响文档状态。</span><span class="sxs-lookup"><span data-stu-id="04074-113">This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but do not need to affect the document state.</span></span>
3. <span data-ttu-id="04074-114">**无会话** - API 调用不传递会话 ID。Excel 服务器必须为每个操作找到服务器的工作簿副本。</span><span class="sxs-lookup"><span data-stu-id="04074-114">**Sessionless**  The API calls do not pass a session Id. The Excel servers have to locate the server's copy of the workbook for each operation.</span></span> <span data-ttu-id="04074-115">这不是调用 Excel API 的有效方式，但它适用于进行某些类型的隔离请求。</span><span class="sxs-lookup"><span data-stu-id="04074-115">This is not an efficient way to call the Excel API, but it is suitable for making certain types of isolated requests.</span></span>

<span data-ttu-id="04074-116">若要表示 API 中的会话，请使用 `workbook-session-id: {session-id}` 标头。</span><span class="sxs-lookup"><span data-stu-id="04074-116">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span>

><span data-ttu-id="04074-p106">**注意：** Excel API 不需要会话标头也能起作用。但是，建议你使用会话标头来提高性能。如果不使用会话标头，API 调用过程中进行的更改_仅_保持在该文件中。</span><span class="sxs-lookup"><span data-stu-id="04074-p106">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="next-step"></a><span data-ttu-id="04074-120">后续步骤</span><span class="sxs-lookup"><span data-stu-id="04074-120">Next step</span></span>
<span data-ttu-id="04074-121">要了解如何创建和使用会话，请参阅[创建会话参考主题](/graph/api/workbook-createsession?view=graph-rest-1.0)。</span><span class="sxs-lookup"><span data-stu-id="04074-121">To learn how to create and use sessions, see the [Create session reference topic](/graph/api/workbook-createsession?view=graph-rest-1.0).</span></span>

## <a name="see-also"></a><span data-ttu-id="04074-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="04074-122">See also</span></span>
* [<span data-ttu-id="04074-123">使用 Microsoft Graph 编写 Excel 工作簿</span><span class="sxs-lookup"><span data-stu-id="04074-123">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="04074-124">通过 Microsoft Graph 使用 Excel 工作簿函数</span><span class="sxs-lookup"><span data-stu-id="04074-124">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="04074-125">通过 Microsoft Graph 更新 Excel 区域的格式</span><span class="sxs-lookup"><span data-stu-id="04074-125">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="04074-126">通过 Microsoft Graph 显示 Excel 图表图像</span><span class="sxs-lookup"><span data-stu-id="04074-126">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="04074-127">使用 Excel REST API</span><span class="sxs-lookup"><span data-stu-id="04074-127">Use the Excel REST API</span></span>](/graph/api/resources/excel?view=graph-rest-1.0)
