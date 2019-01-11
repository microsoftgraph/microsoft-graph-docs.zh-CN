---
title: signInStatus 资源类型
description: 提供的登录状态 （成功或失败） 登录
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878636"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="f9185-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9185-103">signInStatus resource type</span></span>
<span data-ttu-id="f9185-104">提供的登录状态 （成功或失败） 登录</span><span class="sxs-lookup"><span data-stu-id="f9185-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="f9185-105">属性</span><span class="sxs-lookup"><span data-stu-id="f9185-105">Properties</span></span>
| <span data-ttu-id="f9185-106">属性</span><span class="sxs-lookup"><span data-stu-id="f9185-106">Property</span></span>     | <span data-ttu-id="f9185-107">类型</span><span class="sxs-lookup"><span data-stu-id="f9185-107">Type</span></span>   |<span data-ttu-id="f9185-108">Description</span><span class="sxs-lookup"><span data-stu-id="f9185-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9185-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="f9185-109">additionalDetails</span></span>|<span data-ttu-id="f9185-110">字符串</span><span class="sxs-lookup"><span data-stu-id="f9185-110">String</span></span>|<span data-ttu-id="f9185-111">在登录活动上提供的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="f9185-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="f9185-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="f9185-112">errorCode</span></span>|<span data-ttu-id="f9185-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f9185-113">Int32</span></span>|<span data-ttu-id="f9185-114">提供登录故障期间生成的 5 6digit 错误代码。</span><span class="sxs-lookup"><span data-stu-id="f9185-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="f9185-115">签出[的错误代码和消息的列表](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="f9185-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="f9185-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="f9185-116">failureReason</span></span>|<span data-ttu-id="f9185-117">String</span><span class="sxs-lookup"><span data-stu-id="f9185-117">String</span></span>|<span data-ttu-id="f9185-118">提供相应的登录活动的错误消息或失败的原因。</span><span class="sxs-lookup"><span data-stu-id="f9185-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="f9185-119">签出[的错误代码和消息的列表](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="f9185-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9185-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9185-120">JSON representation</span></span>

<span data-ttu-id="f9185-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9185-121">Here is a JSON representation of the resource.</span></span>

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
