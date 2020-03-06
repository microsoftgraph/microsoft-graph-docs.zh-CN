---
title: signInStatus 资源类型
description: 提供登录的登录状态（成功或失败）
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c7880eb89aa4147baa7d8b0bda3aa80d1628bbb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533711"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="ae866-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae866-103">signInStatus resource type</span></span>

<span data-ttu-id="ae866-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae866-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae866-105">提供登录状态（成功或失败）。</span><span class="sxs-lookup"><span data-stu-id="ae866-105">Provides the sign-in status (Success or Failure) of the sign-in.</span></span>

## <a name="properties"></a><span data-ttu-id="ae866-106">属性</span><span class="sxs-lookup"><span data-stu-id="ae866-106">Properties</span></span>

| <span data-ttu-id="ae866-107">属性</span><span class="sxs-lookup"><span data-stu-id="ae866-107">Property</span></span>     | <span data-ttu-id="ae866-108">类型</span><span class="sxs-lookup"><span data-stu-id="ae866-108">Type</span></span>   |<span data-ttu-id="ae866-109">说明</span><span class="sxs-lookup"><span data-stu-id="ae866-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae866-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="ae866-110">additionalDetails</span></span>|<span data-ttu-id="ae866-111">字符串</span><span class="sxs-lookup"><span data-stu-id="ae866-111">String</span></span>|<span data-ttu-id="ae866-112">提供有关登录活动的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="ae866-112">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="ae866-113">errorCode</span><span class="sxs-lookup"><span data-stu-id="ae866-113">errorCode</span></span>|<span data-ttu-id="ae866-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ae866-114">Int32</span></span>|<span data-ttu-id="ae866-115">提供在登录失败过程中生成的 5-6digit 错误代码。</span><span class="sxs-lookup"><span data-stu-id="ae866-115">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="ae866-116">查看[错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="ae866-116">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="ae866-117">failureReason</span><span class="sxs-lookup"><span data-stu-id="ae866-117">failureReason</span></span>|<span data-ttu-id="ae866-118">String</span><span class="sxs-lookup"><span data-stu-id="ae866-118">String</span></span>|<span data-ttu-id="ae866-119">为相应的登录活动提供错误消息或失败原因。</span><span class="sxs-lookup"><span data-stu-id="ae866-119">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="ae866-120">查看[错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="ae866-120">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae866-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae866-121">JSON representation</span></span>

<span data-ttu-id="ae866-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae866-122">Here is a JSON representation of the resource.</span></span>

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
