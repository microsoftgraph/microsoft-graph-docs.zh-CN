---
title: emailActivitySummary 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 039592a33cd004b9a5dc7800c0dbd4ece91bd48c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046882"
---
# <a name="emailactivitysummary-resource-type"></a><span data-ttu-id="20a57-103">emailActivitySummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="20a57-103">emailActivitySummary resource type</span></span>

## <a name="properties"></a><span data-ttu-id="20a57-104">属性</span><span class="sxs-lookup"><span data-stu-id="20a57-104">Properties</span></span>

| <span data-ttu-id="20a57-105">属性</span><span class="sxs-lookup"><span data-stu-id="20a57-105">Property</span></span>          | <span data-ttu-id="20a57-106">类型</span><span class="sxs-lookup"><span data-stu-id="20a57-106">Type</span></span>   |
| :---------------- | :----- |
| <span data-ttu-id="20a57-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="20a57-107">reportRefreshDate</span></span> | <span data-ttu-id="20a57-108">日期</span><span class="sxs-lookup"><span data-stu-id="20a57-108">Date</span></span>   |
| <span data-ttu-id="20a57-109">发送</span><span class="sxs-lookup"><span data-stu-id="20a57-109">send</span></span>              | <span data-ttu-id="20a57-110">Int64</span><span class="sxs-lookup"><span data-stu-id="20a57-110">Int64</span></span>  |
| <span data-ttu-id="20a57-111">接收</span><span class="sxs-lookup"><span data-stu-id="20a57-111">receive</span></span>           | <span data-ttu-id="20a57-112">Int64</span><span class="sxs-lookup"><span data-stu-id="20a57-112">Int64</span></span>  |
| <span data-ttu-id="20a57-113">读取</span><span class="sxs-lookup"><span data-stu-id="20a57-113">read</span></span>              | <span data-ttu-id="20a57-114">Int64</span><span class="sxs-lookup"><span data-stu-id="20a57-114">Int64</span></span>  |
| <span data-ttu-id="20a57-115">reportDate</span><span class="sxs-lookup"><span data-stu-id="20a57-115">reportDate</span></span>        | <span data-ttu-id="20a57-116">日期</span><span class="sxs-lookup"><span data-stu-id="20a57-116">Date</span></span>   |
| <span data-ttu-id="20a57-117">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="20a57-117">reportPeriod</span></span>      | <span data-ttu-id="20a57-118">String</span><span class="sxs-lookup"><span data-stu-id="20a57-118">String</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20a57-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20a57-119">JSON representation</span></span>

<span data-ttu-id="20a57-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20a57-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "send": 1024, 
  "receive": 1024, 
  "read": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
