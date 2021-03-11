---
title: applicationSignInDetailedSummary 资源类型 - Microsoft Graph API
description: 表示应用程序登录的详细摘要。
localization_priority: Normal
author: sureshja
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8f53d1ebce8a7a578c067354ba7f89c6c27ea947
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720828"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="59c61-103">applicationSignInDetailedSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="59c61-103">applicationSignInDetailedSummary resource type</span></span>

<span data-ttu-id="59c61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59c61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59c61-105">表示应用程序登录的详细摘要。</span><span class="sxs-lookup"><span data-stu-id="59c61-105">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="59c61-106">方法</span><span class="sxs-lookup"><span data-stu-id="59c61-106">Methods</span></span>

| <span data-ttu-id="59c61-107">方法</span><span class="sxs-lookup"><span data-stu-id="59c61-107">Method</span></span>       | <span data-ttu-id="59c61-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="59c61-108">Return Type</span></span> | <span data-ttu-id="59c61-109">说明</span><span class="sxs-lookup"><span data-stu-id="59c61-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="59c61-110">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="59c61-110">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="59c61-111">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="59c61-111">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="59c61-112">读取 **applicationSignInDetailedSummary** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59c61-112">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="59c61-113">属性</span><span class="sxs-lookup"><span data-stu-id="59c61-113">Properties</span></span>
| <span data-ttu-id="59c61-114">属性</span><span class="sxs-lookup"><span data-stu-id="59c61-114">Property</span></span>     | <span data-ttu-id="59c61-115">类型</span><span class="sxs-lookup"><span data-stu-id="59c61-115">Type</span></span>        | <span data-ttu-id="59c61-116">说明</span><span class="sxs-lookup"><span data-stu-id="59c61-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59c61-117">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="59c61-117">aggregatedEventDateTime</span></span>|<span data-ttu-id="59c61-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59c61-118">DateTimeOffset</span></span>|<span data-ttu-id="59c61-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="59c61-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="59c61-120">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="59c61-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="59c61-121">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="59c61-121">appDisplayName</span></span>|<span data-ttu-id="59c61-122">String</span><span class="sxs-lookup"><span data-stu-id="59c61-122">String</span></span>|<span data-ttu-id="59c61-123">用户登录的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="59c61-123">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="59c61-124">appId</span><span class="sxs-lookup"><span data-stu-id="59c61-124">appId</span></span>|<span data-ttu-id="59c61-125">String</span><span class="sxs-lookup"><span data-stu-id="59c61-125">String</span></span>|<span data-ttu-id="59c61-126">用户登录的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="59c61-126">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="59c61-127">id</span><span class="sxs-lookup"><span data-stu-id="59c61-127">id</span></span>|<span data-ttu-id="59c61-128">String</span><span class="sxs-lookup"><span data-stu-id="59c61-128">String</span></span>| <span data-ttu-id="59c61-129">表示登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="59c61-129">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="59c61-130">signInCount</span><span class="sxs-lookup"><span data-stu-id="59c61-130">signInCount</span></span>|<span data-ttu-id="59c61-131">Int64</span><span class="sxs-lookup"><span data-stu-id="59c61-131">Int64</span></span>|<span data-ttu-id="59c61-132">应用程序进行登录的计数。</span><span class="sxs-lookup"><span data-stu-id="59c61-132">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="59c61-133">status</span><span class="sxs-lookup"><span data-stu-id="59c61-133">status</span></span>|[<span data-ttu-id="59c61-134">signInStatus</span><span class="sxs-lookup"><span data-stu-id="59c61-134">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="59c61-135">登录状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="59c61-135">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59c61-136">关系</span><span class="sxs-lookup"><span data-stu-id="59c61-136">Relationships</span></span>
<span data-ttu-id="59c61-137">无</span><span class="sxs-lookup"><span data-stu-id="59c61-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="59c61-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59c61-138">JSON representation</span></span>

<span data-ttu-id="59c61-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59c61-139">The following is a JSON representation of the resource.</span></span>

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


