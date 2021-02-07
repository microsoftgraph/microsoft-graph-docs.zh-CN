---
title: signInStatus 资源类型
description: 提供登录状态 (登录成功) 失败状态
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 37eb91434fd7a5fb0dc65f5c7203effd42f3878e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137086"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="ad669-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad669-103">signInStatus resource type</span></span>

<span data-ttu-id="ad669-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad669-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad669-105">提供登录状态 (登录的成功) 失败状态。</span><span class="sxs-lookup"><span data-stu-id="ad669-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="ad669-106">属性</span><span class="sxs-lookup"><span data-stu-id="ad669-106">Properties</span></span>

| <span data-ttu-id="ad669-107">属性</span><span class="sxs-lookup"><span data-stu-id="ad669-107">Property</span></span>     | <span data-ttu-id="ad669-108">类型</span><span class="sxs-lookup"><span data-stu-id="ad669-108">Type</span></span>   |<span data-ttu-id="ad669-109">说明</span><span class="sxs-lookup"><span data-stu-id="ad669-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad669-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="ad669-110">additionalDetails</span></span>|<span data-ttu-id="ad669-111">String</span><span class="sxs-lookup"><span data-stu-id="ad669-111">String</span></span>|<span data-ttu-id="ad669-112">提供有关登录活动的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="ad669-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="ad669-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="ad669-113">errorCode</span></span>|<span data-ttu-id="ad669-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ad669-114">Int32</span></span>|<span data-ttu-id="ad669-115">提供登录失败期间生成的 5-6 位数字错误代码。</span><span class="sxs-lookup"><span data-stu-id="ad669-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="ad669-116">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="ad669-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="ad669-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="ad669-117">failureReason</span></span>|<span data-ttu-id="ad669-118">String</span><span class="sxs-lookup"><span data-stu-id="ad669-118">String</span></span>|<span data-ttu-id="ad669-119">提供相应登录活动的错误消息或失败原因。</span><span class="sxs-lookup"><span data-stu-id="ad669-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="ad669-120">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="ad669-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ad669-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad669-121">JSON representation</span></span>

<span data-ttu-id="ad669-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad669-122">Here is a JSON representation of the resource.</span></span>

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

