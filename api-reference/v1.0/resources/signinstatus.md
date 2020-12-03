---
title: signInStatus 资源类型
description: 提供登录状态 (成功或失败) 登录
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3633968869c0cf61e16afa4ba056a530c86b3c93
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563651"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="f84a5-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f84a5-103">signInStatus resource type</span></span>

<span data-ttu-id="f84a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f84a5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f84a5-105">提供登录状态 (成功或失败) 。</span><span class="sxs-lookup"><span data-stu-id="f84a5-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="f84a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="f84a5-106">Properties</span></span>

| <span data-ttu-id="f84a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="f84a5-107">Property</span></span>     | <span data-ttu-id="f84a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="f84a5-108">Type</span></span>   |<span data-ttu-id="f84a5-109">说明</span><span class="sxs-lookup"><span data-stu-id="f84a5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f84a5-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="f84a5-110">additionalDetails</span></span>|<span data-ttu-id="f84a5-111">String</span><span class="sxs-lookup"><span data-stu-id="f84a5-111">String</span></span>|<span data-ttu-id="f84a5-112">提供有关登录活动的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="f84a5-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="f84a5-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="f84a5-113">errorCode</span></span>|<span data-ttu-id="f84a5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f84a5-114">Int32</span></span>|<span data-ttu-id="f84a5-115">提供在登录失败过程中生成的5-6 位错误代码。</span><span class="sxs-lookup"><span data-stu-id="f84a5-115">Provides the 5-6 digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="f84a5-116">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="f84a5-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="f84a5-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="f84a5-117">failureReason</span></span>|<span data-ttu-id="f84a5-118">String</span><span class="sxs-lookup"><span data-stu-id="f84a5-118">String</span></span>|<span data-ttu-id="f84a5-119">为相应的登录活动提供错误消息或失败原因。</span><span class="sxs-lookup"><span data-stu-id="f84a5-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="f84a5-120">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="f84a5-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f84a5-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f84a5-121">JSON representation</span></span>

<span data-ttu-id="f84a5-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f84a5-122">Here is a JSON representation of the resource.</span></span>

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

