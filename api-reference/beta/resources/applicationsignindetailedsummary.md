---
title: applicationSignInDetailedSummary 资源类型-Microsoft Graph API
description: 表示应用程序登录的详细摘要。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 118d26e6d46e5b64861a041eec12d03bea533552
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508273"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="692e4-103">applicationSignInDetailedSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="692e4-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="692e4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="692e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="692e4-105">表示应用程序登录的详细摘要。</span><span class="sxs-lookup"><span data-stu-id="692e4-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="692e4-106">方法</span><span class="sxs-lookup"><span data-stu-id="692e4-106">Methods</span></span>

| <span data-ttu-id="692e4-107">方法</span><span class="sxs-lookup"><span data-stu-id="692e4-107">Method</span></span>       | <span data-ttu-id="692e4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="692e4-108">Return Type</span></span> | <span data-ttu-id="692e4-109">说明</span><span class="sxs-lookup"><span data-stu-id="692e4-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="692e4-110">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="692e4-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="692e4-111">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="692e4-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="692e4-112">读取**applicationSignInDetailedSummary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="692e4-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="692e4-113">属性</span><span class="sxs-lookup"><span data-stu-id="692e4-113">Properties</span></span>
| <span data-ttu-id="692e4-114">属性</span><span class="sxs-lookup"><span data-stu-id="692e4-114">Property</span></span>     | <span data-ttu-id="692e4-115">类型</span><span class="sxs-lookup"><span data-stu-id="692e4-115">Type</span></span>        | <span data-ttu-id="692e4-116">说明</span><span class="sxs-lookup"><span data-stu-id="692e4-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="692e4-117">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="692e4-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="692e4-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="692e4-118">DateTimeOffset</span></span>|<span data-ttu-id="692e4-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="692e4-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="692e4-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="692e4-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="692e4-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="692e4-121">appDisplayName</span></span>|<span data-ttu-id="692e4-122">String</span><span class="sxs-lookup"><span data-stu-id="692e4-122">String</span></span>|<span data-ttu-id="692e4-123">用户登录到的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="692e4-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="692e4-124">appId</span><span class="sxs-lookup"><span data-stu-id="692e4-124">appId</span></span>|<span data-ttu-id="692e4-125">String</span><span class="sxs-lookup"><span data-stu-id="692e4-125">String</span></span>|<span data-ttu-id="692e4-126">用户登录到的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="692e4-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="692e4-127">id</span><span class="sxs-lookup"><span data-stu-id="692e4-127">id</span></span>|<span data-ttu-id="692e4-128">字符串</span><span class="sxs-lookup"><span data-stu-id="692e4-128">String</span></span>| <span data-ttu-id="692e4-129">一个代表登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="692e4-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="692e4-130">signInCount</span><span class="sxs-lookup"><span data-stu-id="692e4-130">signInCount</span></span>|<span data-ttu-id="692e4-131">Int64</span><span class="sxs-lookup"><span data-stu-id="692e4-131">Int64</span></span>|<span data-ttu-id="692e4-132">应用程序发出的登录数。</span><span class="sxs-lookup"><span data-stu-id="692e4-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="692e4-133">status</span><span class="sxs-lookup"><span data-stu-id="692e4-133">status</span></span>|[<span data-ttu-id="692e4-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="692e4-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="692e4-135">登录状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="692e4-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="692e4-136">关系</span><span class="sxs-lookup"><span data-stu-id="692e4-136">Relationships</span></span>
<span data-ttu-id="692e4-137">无</span><span class="sxs-lookup"><span data-stu-id="692e4-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="692e4-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="692e4-138">JSON representation</span></span>

<span data-ttu-id="692e4-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="692e4-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
}-->

```json
{
  "aggregatedEventDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "id": "String (identifier)",
  "signInCount": 1024,
  "status": {"@odata.type": "microsoft.graph.signInStatus"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInDetailedSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
