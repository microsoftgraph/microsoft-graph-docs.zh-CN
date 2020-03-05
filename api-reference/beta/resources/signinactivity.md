---
title: signInActivity 资源类型
description: 提供特定用户的上次登录日期。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8144a681f93df45827c8b304d507eea820adcca2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520595"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="e75d8-103">signInActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="e75d8-103">signInActivity resource type</span></span>

<span data-ttu-id="e75d8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e75d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e75d8-105">提供特定用户的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="e75d8-105">Provides the last signed-in date for a specific user.</span></span>

## <a name="properties"></a><span data-ttu-id="e75d8-106">属性</span><span class="sxs-lookup"><span data-stu-id="e75d8-106">Properties</span></span>

| <span data-ttu-id="e75d8-107">属性</span><span class="sxs-lookup"><span data-stu-id="e75d8-107">Property</span></span>     | <span data-ttu-id="e75d8-108">类型</span><span class="sxs-lookup"><span data-stu-id="e75d8-108">Type</span></span>        | <span data-ttu-id="e75d8-109">说明</span><span class="sxs-lookup"><span data-stu-id="e75d8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e75d8-110">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="e75d8-110">lastSignInDateTime</span></span>|<span data-ttu-id="e75d8-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e75d8-111">DateTimeOffset</span></span>|<span data-ttu-id="e75d8-112">特定用户的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="e75d8-112">The last sign-in date for a specific user.</span></span> <span data-ttu-id="e75d8-113">您可以使用此字段来计算用户上次登录目录的时间。</span><span class="sxs-lookup"><span data-stu-id="e75d8-113">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="e75d8-114">此字段可用于生成报表，如非活动用户。</span><span class="sxs-lookup"><span data-stu-id="e75d8-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="e75d8-115">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="e75d8-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e75d8-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="e75d8-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e75d8-117">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="e75d8-117">lastSignInRequestId</span></span>|<span data-ttu-id="e75d8-118">String</span><span class="sxs-lookup"><span data-stu-id="e75d8-118">String</span></span>|<span data-ttu-id="e75d8-119">此用户执行的最后一个登录的请求 ID。</span><span class="sxs-lookup"><span data-stu-id="e75d8-119">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e75d8-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e75d8-120">JSON representation</span></span>

<span data-ttu-id="e75d8-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e75d8-121">The following is a JSON representation of the resource.</span></span>

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