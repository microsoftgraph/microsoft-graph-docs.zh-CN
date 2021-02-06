---
title: signInStatus 资源类型
description: 提供登录状态 (登录成功) 失败状态
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: d7428c2a73d0b4a114599dad8ac1740d91ba5865
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132634"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="1c3a9-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c3a9-103">signInStatus resource type</span></span>

<span data-ttu-id="1c3a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c3a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c3a9-105">提供登录状态 (登录成功) 失败状态</span><span class="sxs-lookup"><span data-stu-id="1c3a9-105">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="1c3a9-106">属性</span><span class="sxs-lookup"><span data-stu-id="1c3a9-106">Properties</span></span>
| <span data-ttu-id="1c3a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c3a9-107">Property</span></span>     | <span data-ttu-id="1c3a9-108">类型</span><span class="sxs-lookup"><span data-stu-id="1c3a9-108">Type</span></span>   |<span data-ttu-id="1c3a9-109">说明</span><span class="sxs-lookup"><span data-stu-id="1c3a9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c3a9-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="1c3a9-110">additionalDetails</span></span>|<span data-ttu-id="1c3a9-111">字符串</span><span class="sxs-lookup"><span data-stu-id="1c3a9-111">String</span></span>|<span data-ttu-id="1c3a9-112">提供有关登录活动的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="1c3a9-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="1c3a9-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="1c3a9-113">errorCode</span></span>|<span data-ttu-id="1c3a9-114">Int32</span><span class="sxs-lookup"><span data-stu-id="1c3a9-114">Int32</span></span>|<span data-ttu-id="1c3a9-115">提供登录失败期间生成的 5-6 位数字错误代码。</span><span class="sxs-lookup"><span data-stu-id="1c3a9-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="1c3a9-116">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="1c3a9-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="1c3a9-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="1c3a9-117">failureReason</span></span>|<span data-ttu-id="1c3a9-118">String</span><span class="sxs-lookup"><span data-stu-id="1c3a9-118">String</span></span>|<span data-ttu-id="1c3a9-119">提供相应登录活动的错误消息或失败原因。</span><span class="sxs-lookup"><span data-stu-id="1c3a9-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="1c3a9-120">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="1c3a9-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c3a9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c3a9-121">JSON representation</span></span>

<span data-ttu-id="1c3a9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c3a9-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


