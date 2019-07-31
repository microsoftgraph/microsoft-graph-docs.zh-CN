---
title: applicationSignInDetailedSummary 资源类型-Microsoft Graph API
description: 表示应用程序登录的详细摘要。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 527d60ff025e9a6d081226a51ec8cbefc53c20de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013328"
---
# <a name="applicationsignindetailedsummary-resource-type"></a><span data-ttu-id="13204-103">applicationSignInDetailedSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="13204-103">applicationSignInDetailedSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13204-104">表示应用程序登录的详细摘要。</span><span class="sxs-lookup"><span data-stu-id="13204-104">Represents a detailed summary of an application sign-in.</span></span>

## <a name="methods"></a><span data-ttu-id="13204-105">方法</span><span class="sxs-lookup"><span data-stu-id="13204-105">Methods</span></span>

| <span data-ttu-id="13204-106">方法</span><span class="sxs-lookup"><span data-stu-id="13204-106">Method</span></span>       | <span data-ttu-id="13204-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="13204-107">Return Type</span></span> | <span data-ttu-id="13204-108">说明</span><span class="sxs-lookup"><span data-stu-id="13204-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="13204-109">获取 applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="13204-109">Get applicationSignInDetailedSummary</span></span>](../api/applicationsignindetailedsummary-get.md) | [<span data-ttu-id="13204-110">applicationSignInDetailedSummary</span><span class="sxs-lookup"><span data-stu-id="13204-110">applicationSignInDetailedSummary</span></span>](applicationsignindetailedsummary.md) | <span data-ttu-id="13204-111">读取**applicationSignInDetailedSummary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="13204-111">Read the properties and relationships of an **applicationSignInDetailedSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="13204-112">属性</span><span class="sxs-lookup"><span data-stu-id="13204-112">Properties</span></span>
| <span data-ttu-id="13204-113">属性</span><span class="sxs-lookup"><span data-stu-id="13204-113">Property</span></span>     | <span data-ttu-id="13204-114">类型</span><span class="sxs-lookup"><span data-stu-id="13204-114">Type</span></span>        | <span data-ttu-id="13204-115">说明</span><span class="sxs-lookup"><span data-stu-id="13204-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13204-116">aggregatedEventDateTime</span><span class="sxs-lookup"><span data-stu-id="13204-116">aggregatedEventDateTime</span></span>|<span data-ttu-id="13204-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13204-117">DateTimeOffset</span></span>|<span data-ttu-id="13204-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="13204-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13204-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="13204-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="13204-120">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="13204-120">appDisplayName</span></span>|<span data-ttu-id="13204-121">String</span><span class="sxs-lookup"><span data-stu-id="13204-121">String</span></span>|<span data-ttu-id="13204-122">用户登录到的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="13204-122">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="13204-123">appId</span><span class="sxs-lookup"><span data-stu-id="13204-123">appId</span></span>|<span data-ttu-id="13204-124">String</span><span class="sxs-lookup"><span data-stu-id="13204-124">String</span></span>|<span data-ttu-id="13204-125">用户登录到的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="13204-125">ID of the application that the user signed in to.</span></span>|
|<span data-ttu-id="13204-126">id</span><span class="sxs-lookup"><span data-stu-id="13204-126">id</span></span>|<span data-ttu-id="13204-127">字符串</span><span class="sxs-lookup"><span data-stu-id="13204-127">String</span></span>| <span data-ttu-id="13204-128">一个代表登录活动的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="13204-128">A unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="13204-129">signInCount</span><span class="sxs-lookup"><span data-stu-id="13204-129">signInCount</span></span>|<span data-ttu-id="13204-130">Int64</span><span class="sxs-lookup"><span data-stu-id="13204-130">Int64</span></span>|<span data-ttu-id="13204-131">应用程序发出的登录数。</span><span class="sxs-lookup"><span data-stu-id="13204-131">Count of sign-ins made by the application.</span></span>|
|<span data-ttu-id="13204-132">status</span><span class="sxs-lookup"><span data-stu-id="13204-132">status</span></span>|[<span data-ttu-id="13204-133">signInStatus</span><span class="sxs-lookup"><span data-stu-id="13204-133">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="13204-134">登录状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="13204-134">Details of the sign-in status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13204-135">关系</span><span class="sxs-lookup"><span data-stu-id="13204-135">Relationships</span></span>
<span data-ttu-id="13204-136">无</span><span class="sxs-lookup"><span data-stu-id="13204-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="13204-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13204-137">JSON representation</span></span>

<span data-ttu-id="13204-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13204-138">The following is a JSON representation of the resource.</span></span>

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
