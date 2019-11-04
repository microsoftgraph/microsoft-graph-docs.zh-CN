---
title: signInActivity 资源类型
description: 提供特定用户的上次登录日期。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d93ff4f3b395d9b0820865c3293a419471ab6473
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939241"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="fb374-103">signInActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb374-103">signInActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb374-104">提供特定用户的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="fb374-104">Provides the last signed-in date for a specific user.</span></span>

## <a name="properties"></a><span data-ttu-id="fb374-105">属性</span><span class="sxs-lookup"><span data-stu-id="fb374-105">Properties</span></span>

| <span data-ttu-id="fb374-106">属性</span><span class="sxs-lookup"><span data-stu-id="fb374-106">Property</span></span>     | <span data-ttu-id="fb374-107">类型</span><span class="sxs-lookup"><span data-stu-id="fb374-107">Type</span></span>        | <span data-ttu-id="fb374-108">描述</span><span class="sxs-lookup"><span data-stu-id="fb374-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fb374-109">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="fb374-109">lastSignInDateTime</span></span>|<span data-ttu-id="fb374-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb374-110">DateTimeOffset</span></span>|<span data-ttu-id="fb374-111">特定用户的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="fb374-111">The last sign-in date for a specific user.</span></span> <span data-ttu-id="fb374-112">您可以使用此字段来计算用户上次登录目录的时间。</span><span class="sxs-lookup"><span data-stu-id="fb374-112">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="fb374-113">此字段可用于生成报表，如非活动用户。</span><span class="sxs-lookup"><span data-stu-id="fb374-113">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="fb374-114">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="fb374-114">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fb374-115">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="fb374-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="fb374-116">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="fb374-116">lastSignInRequestId</span></span>|<span data-ttu-id="fb374-117">字符串</span><span class="sxs-lookup"><span data-stu-id="fb374-117">String</span></span>|<span data-ttu-id="fb374-118">此用户执行的最后一个登录的请求 ID。</span><span class="sxs-lookup"><span data-stu-id="fb374-118">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb374-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb374-119">JSON representation</span></span>

<span data-ttu-id="fb374-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb374-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->