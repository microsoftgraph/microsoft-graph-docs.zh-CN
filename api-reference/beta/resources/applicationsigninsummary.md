---
title: applicationSignInDetailedSummary 资源类型
description: 表示应用程序登录摘要。
localization_priority: Normal
author: kholtz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 79dbe02f723c9c8912ce8a227a47d6f50260c330
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455274"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="942a0-103">applicationSignInSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="942a0-103">applicationSignInSummary resource type</span></span>

<span data-ttu-id="942a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="942a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="942a0-105">表示应用程序登录摘要。</span><span class="sxs-lookup"><span data-stu-id="942a0-105">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="942a0-106">方法</span><span class="sxs-lookup"><span data-stu-id="942a0-106">Methods</span></span>

| <span data-ttu-id="942a0-107">方法</span><span class="sxs-lookup"><span data-stu-id="942a0-107">Method</span></span>       | <span data-ttu-id="942a0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="942a0-108">Return Type</span></span> | <span data-ttu-id="942a0-109">说明</span><span class="sxs-lookup"><span data-stu-id="942a0-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="942a0-110">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="942a0-110">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="942a0-111">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="942a0-111">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="942a0-112">读取**applicationSignInSummary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="942a0-112">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="942a0-113">属性</span><span class="sxs-lookup"><span data-stu-id="942a0-113">Properties</span></span>
| <span data-ttu-id="942a0-114">属性</span><span class="sxs-lookup"><span data-stu-id="942a0-114">Property</span></span>     | <span data-ttu-id="942a0-115">类型</span><span class="sxs-lookup"><span data-stu-id="942a0-115">Type</span></span>        | <span data-ttu-id="942a0-116">说明</span><span class="sxs-lookup"><span data-stu-id="942a0-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="942a0-117">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="942a0-117">appDisplayName</span></span>|<span data-ttu-id="942a0-118">String</span><span class="sxs-lookup"><span data-stu-id="942a0-118">String</span></span>|<span data-ttu-id="942a0-119">用户登录到的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="942a0-119">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="942a0-120">appId</span><span class="sxs-lookup"><span data-stu-id="942a0-120">appId</span></span>|<span data-ttu-id="942a0-121">String</span><span class="sxs-lookup"><span data-stu-id="942a0-121">String</span></span>|  <span data-ttu-id="942a0-122">用户签署的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="942a0-122">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="942a0-123">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="942a0-123">failedSignInCount</span></span>|<span data-ttu-id="942a0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="942a0-124">Int64</span></span>|<span data-ttu-id="942a0-125">应用程序发出的失败登录数。</span><span class="sxs-lookup"><span data-stu-id="942a0-125">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="942a0-126">successPercentage</span><span class="sxs-lookup"><span data-stu-id="942a0-126">successPercentage</span></span>|<span data-ttu-id="942a0-127">Int32</span><span class="sxs-lookup"><span data-stu-id="942a0-127">Int32</span></span>|<span data-ttu-id="942a0-128">由应用程序成功登录所占的百分比。</span><span class="sxs-lookup"><span data-stu-id="942a0-128">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="942a0-129">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="942a0-129">successfulSignInCount</span></span>|<span data-ttu-id="942a0-130">Int64</span><span class="sxs-lookup"><span data-stu-id="942a0-130">Int64</span></span>|<span data-ttu-id="942a0-131">应用程序成功登录时所用的计数。</span><span class="sxs-lookup"><span data-stu-id="942a0-131">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="942a0-132">关系</span><span class="sxs-lookup"><span data-stu-id="942a0-132">Relationships</span></span>
<span data-ttu-id="942a0-133">无</span><span class="sxs-lookup"><span data-stu-id="942a0-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="942a0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="942a0-134">JSON representation</span></span>

<span data-ttu-id="942a0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="942a0-135">The following is a JSON representation of the resource.</span></span>

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
