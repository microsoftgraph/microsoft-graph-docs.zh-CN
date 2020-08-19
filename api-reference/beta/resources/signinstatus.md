---
title: signInStatus 资源类型
description: 提供登录状态 (成功或失败) 登录
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: SarahBar
ms.openlocfilehash: 7cb48f7a4235b28231ab93fc3ccfba074f80d286
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808597"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="3c3fe-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="3c3fe-103">signInStatus resource type</span></span>

<span data-ttu-id="3c3fe-104">命名空间： microsoft. graph 提供登录状态 (成功或失败) 登录</span><span class="sxs-lookup"><span data-stu-id="3c3fe-104">Namespace: microsoft.graph Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="3c3fe-105">属性</span><span class="sxs-lookup"><span data-stu-id="3c3fe-105">Properties</span></span>
| <span data-ttu-id="3c3fe-106">属性</span><span class="sxs-lookup"><span data-stu-id="3c3fe-106">Property</span></span>     | <span data-ttu-id="3c3fe-107">类型</span><span class="sxs-lookup"><span data-stu-id="3c3fe-107">Type</span></span>   |<span data-ttu-id="3c3fe-108">说明</span><span class="sxs-lookup"><span data-stu-id="3c3fe-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c3fe-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="3c3fe-109">additionalDetails</span></span>|<span data-ttu-id="3c3fe-110">String</span><span class="sxs-lookup"><span data-stu-id="3c3fe-110">String</span></span>|<span data-ttu-id="3c3fe-111">提供有关登录活动的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="3c3fe-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="3c3fe-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="3c3fe-112">errorCode</span></span>|<span data-ttu-id="3c3fe-113">Int32</span><span class="sxs-lookup"><span data-stu-id="3c3fe-113">Int32</span></span>|<span data-ttu-id="3c3fe-114">提供在登录失败过程中生成的 5-6digit 错误代码。</span><span class="sxs-lookup"><span data-stu-id="3c3fe-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="3c3fe-115">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="3c3fe-115">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="3c3fe-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="3c3fe-116">failureReason</span></span>|<span data-ttu-id="3c3fe-117">String</span><span class="sxs-lookup"><span data-stu-id="3c3fe-117">String</span></span>|<span data-ttu-id="3c3fe-118">为相应的登录活动提供错误消息或失败原因。</span><span class="sxs-lookup"><span data-stu-id="3c3fe-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="3c3fe-119">查看 [错误代码和消息的列表](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="3c3fe-119">Check out the [list of error codes and messages](/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c3fe-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3c3fe-120">JSON representation</span></span>

<span data-ttu-id="3c3fe-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c3fe-121">Here is a JSON representation of the resource.</span></span>

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
