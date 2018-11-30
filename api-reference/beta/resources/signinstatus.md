---
title: signInStatus 资源类型
description: 提供的登录状态 （成功或失败） 登录
ms.openlocfilehash: cafa0dffe1b1d798d87225ac82901cf041d5e4fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048319"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="c4c62-103">signInStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4c62-103">signInStatus resource type</span></span>
<span data-ttu-id="c4c62-104">提供的登录状态 （成功或失败） 登录</span><span class="sxs-lookup"><span data-stu-id="c4c62-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="c4c62-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4c62-105">Properties</span></span>
| <span data-ttu-id="c4c62-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4c62-106">Property</span></span>     | <span data-ttu-id="c4c62-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4c62-107">Type</span></span>   |<span data-ttu-id="c4c62-108">说明</span><span class="sxs-lookup"><span data-stu-id="c4c62-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4c62-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="c4c62-109">additionalDetails</span></span>|<span data-ttu-id="c4c62-110">字符串</span><span class="sxs-lookup"><span data-stu-id="c4c62-110">String</span></span>|<span data-ttu-id="c4c62-111">在登录活动上提供的其他详细信息</span><span class="sxs-lookup"><span data-stu-id="c4c62-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="c4c62-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="c4c62-112">errorCode</span></span>|<span data-ttu-id="c4c62-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c4c62-113">Int32</span></span>|<span data-ttu-id="c4c62-114">提供登录故障期间生成的 5 6digit 错误代码。</span><span class="sxs-lookup"><span data-stu-id="c4c62-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="c4c62-115">签出[的错误代码和消息的列表](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="c4c62-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="c4c62-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="c4c62-116">failureReason</span></span>|<span data-ttu-id="c4c62-117">String</span><span class="sxs-lookup"><span data-stu-id="c4c62-117">String</span></span>|<span data-ttu-id="c4c62-118">提供相应的登录活动的错误消息或失败的原因。</span><span class="sxs-lookup"><span data-stu-id="c4c62-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="c4c62-119">签出[的错误代码和消息的列表](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)。</span><span class="sxs-lookup"><span data-stu-id="c4c62-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4c62-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4c62-120">JSON representation</span></span>

<span data-ttu-id="c4c62-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4c62-121">Here is a JSON representation of the resource.</span></span>

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