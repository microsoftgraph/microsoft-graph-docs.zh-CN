---
title: Microsoft Graph 中的云通信 API 限制
description: 这包含有关云通信 Api 限制的信息
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 0338c7b37a58da66aac75430234a4b1df56b07b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871575"
---
# <a name="cloud-communication-api-limits-in-microsoft-graph"></a><span data-ttu-id="7e281-103">Microsoft Graph 中的云通信 API 限制</span><span class="sxs-lookup"><span data-stu-id="7e281-103">Cloud communication API limits in Microsoft Graph</span></span>

<span data-ttu-id="7e281-104">本文介绍了云通信 Api 的限制。</span><span class="sxs-lookup"><span data-stu-id="7e281-104">This article describes limitations to the cloud communications APIs.</span></span> <span data-ttu-id="7e281-105">这些限制有助于确保平台的稳定性、可靠性和安全性。</span><span class="sxs-lookup"><span data-stu-id="7e281-105">These limits help to ensure that the platform is stable, reliable, and secure.</span></span> <span data-ttu-id="7e281-106">请注意，这些限制可能会在将来发生更改。</span><span class="sxs-lookup"><span data-stu-id="7e281-106">Note that these limitations are subject to change in the future.</span></span> 

><span data-ttu-id="7e281-107">**注意：** 当达到限制时，尝试生成更多的 API 请求将导致出现 HTTP `429 Error`。</span><span class="sxs-lookup"><span data-stu-id="7e281-107">**Note:** When the limit is reached, attempting to make more API requests will result in an HTTP `429 Error`.</span></span>

| <span data-ttu-id="7e281-108">API</span><span class="sxs-lookup"><span data-stu-id="7e281-108">API</span></span>      | <span data-ttu-id="7e281-109">限制</span><span class="sxs-lookup"><span data-stu-id="7e281-109">Limitations</span></span>    |
| :------------- | :----------: |
|  <span data-ttu-id="7e281-110">呼叫</span><span class="sxs-lookup"><span data-stu-id="7e281-110">Calls</span></span> | <span data-ttu-id="7e281-111">10000呼叫/月和100并发呼叫</span><span class="sxs-lookup"><span data-stu-id="7e281-111">10,000 calls/month and 100 concurrent calls</span></span>   |
| <span data-ttu-id="7e281-112">会议</span><span class="sxs-lookup"><span data-stu-id="7e281-112">Meetings</span></span>   | <span data-ttu-id="7e281-113">每月2000会议/用户</span><span class="sxs-lookup"><span data-stu-id="7e281-113">2000 meetings/user each month</span></span> |
| <span data-ttu-id="7e281-114">状态（预览）</span><span class="sxs-lookup"><span data-stu-id="7e281-114">Presence (preview)</span></span>   | <span data-ttu-id="7e281-115">每秒2个请求</span><span class="sxs-lookup"><span data-stu-id="7e281-115">2 requests/second</span></span> |

## <a name="see-also"></a><span data-ttu-id="7e281-116">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7e281-116">See also</span></span>

- [<span data-ttu-id="7e281-117">使用通信 API</span><span class="sxs-lookup"><span data-stu-id="7e281-117">Working with the communications API</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-beta)
