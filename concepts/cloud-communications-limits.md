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
# <a name="cloud-communication-api-limits-in-microsoft-graph"></a>Microsoft Graph 中的云通信 API 限制

本文介绍了云通信 Api 的限制。 这些限制有助于确保平台的稳定性、可靠性和安全性。 请注意，这些限制可能会在将来发生更改。 

>**注意：** 当达到限制时，尝试生成更多的 API 请求将导致出现 HTTP `429 Error`。

| API      | 限制    |
| :------------- | :----------: |
|  呼叫 | 10000呼叫/月和100并发呼叫   |
| 会议   | 每月2000会议/用户 |
| 状态（预览）   | 每秒2个请求 |

## <a name="see-also"></a>另请参阅

- [使用通信 API](/graph/api/resources/communications-api-overview?view=graph-rest-beta)
