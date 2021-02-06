---
title: applicationSignInDetailedSummary 资源类型
description: 表示应用程序登录摘要。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 454c4e2e9e57b61194e6f3e6970e5db1ea414369
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137408"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="4f7c5-103">applicationSignInSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f7c5-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="4f7c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f7c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f7c5-105">表示应用程序登录摘要。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="4f7c5-106">方法</span><span class="sxs-lookup"><span data-stu-id="4f7c5-106">Methods</span></span>

| <span data-ttu-id="4f7c5-107">方法</span><span class="sxs-lookup"><span data-stu-id="4f7c5-107">Method</span></span>       | <span data-ttu-id="4f7c5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4f7c5-108">Return Type</span></span> | <span data-ttu-id="4f7c5-109">说明</span><span class="sxs-lookup"><span data-stu-id="4f7c5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4f7c5-110">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="4f7c5-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="4f7c5-111">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="4f7c5-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="4f7c5-112">读取 **applicationSignInSummary** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4f7c5-113">属性</span><span class="sxs-lookup"><span data-stu-id="4f7c5-113">Properties</span></span>
| <span data-ttu-id="4f7c5-114">属性</span><span class="sxs-lookup"><span data-stu-id="4f7c5-114">Property</span></span>     | <span data-ttu-id="4f7c5-115">类型</span><span class="sxs-lookup"><span data-stu-id="4f7c5-115">Type</span></span>        | <span data-ttu-id="4f7c5-116">说明</span><span class="sxs-lookup"><span data-stu-id="4f7c5-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f7c5-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4f7c5-117">appDisplayName</span></span>|<span data-ttu-id="4f7c5-118">String</span><span class="sxs-lookup"><span data-stu-id="4f7c5-118">String</span></span>|<span data-ttu-id="4f7c5-119">用户登录的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="4f7c5-120">appId</span><span class="sxs-lookup"><span data-stu-id="4f7c5-120">appId</span></span>|<span data-ttu-id="4f7c5-121">String</span><span class="sxs-lookup"><span data-stu-id="4f7c5-121">String</span></span>|  <span data-ttu-id="4f7c5-122">用户签名 i nto 的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="4f7c5-123">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="4f7c5-123">failedSignInCount</span></span>|<span data-ttu-id="4f7c5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="4f7c5-124">Int64</span></span>|<span data-ttu-id="4f7c5-125">应用程序进行失败登录的计数。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="4f7c5-126">successPercentage</span><span class="sxs-lookup"><span data-stu-id="4f7c5-126">successPercentage</span></span>|<span data-ttu-id="4f7c5-127">Int32</span><span class="sxs-lookup"><span data-stu-id="4f7c5-127">Int32</span></span>|<span data-ttu-id="4f7c5-128">应用程序成功登录的百分比。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="4f7c5-129">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="4f7c5-129">successfulSignInCount</span></span>|<span data-ttu-id="4f7c5-130">Int64</span><span class="sxs-lookup"><span data-stu-id="4f7c5-130">Int64</span></span>|<span data-ttu-id="4f7c5-131">应用程序成功登录的计数。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f7c5-132">关系</span><span class="sxs-lookup"><span data-stu-id="4f7c5-132">Relationships</span></span>
<span data-ttu-id="4f7c5-133">无</span><span class="sxs-lookup"><span data-stu-id="4f7c5-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4f7c5-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f7c5-134">JSON representation</span></span>

<span data-ttu-id="4f7c5-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f7c5-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationSignInSummary"
}-->

```json
{
  "appDisplayName": "String",
  "appId": "String (identifier)",
  "failedSignInCount": 1024,
  "successPercentage": 1024,
  "successfulSignInCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationSignInSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


