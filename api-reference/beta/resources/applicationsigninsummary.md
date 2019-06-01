---
title: applicationSignInDetailedSummary 资源类型
description: 表示应用程序登录摘要。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c6ecd91bb29abc409a745e92b523948b78552ed4
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657621"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="e7316-103">applicationSignInSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7316-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7316-104">表示应用程序登录摘要。</span><span class="sxs-lookup"><span data-stu-id="e7316-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="e7316-105">方法</span><span class="sxs-lookup"><span data-stu-id="e7316-105">Methods</span></span>

| <span data-ttu-id="e7316-106">方法</span><span class="sxs-lookup"><span data-stu-id="e7316-106">Method</span></span>       | <span data-ttu-id="e7316-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7316-107">Return Type</span></span> | <span data-ttu-id="e7316-108">说明</span><span class="sxs-lookup"><span data-stu-id="e7316-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7316-109">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="e7316-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="e7316-110">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="e7316-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="e7316-111">读取**applicationSignInSummary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7316-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e7316-112">属性</span><span class="sxs-lookup"><span data-stu-id="e7316-112">Properties</span></span>
| <span data-ttu-id="e7316-113">属性</span><span class="sxs-lookup"><span data-stu-id="e7316-113">Property</span></span>     | <span data-ttu-id="e7316-114">类型</span><span class="sxs-lookup"><span data-stu-id="e7316-114">Type</span></span>        | <span data-ttu-id="e7316-115">说明</span><span class="sxs-lookup"><span data-stu-id="e7316-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7316-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7316-116">appDisplayName</span></span>|<span data-ttu-id="e7316-117">String</span><span class="sxs-lookup"><span data-stu-id="e7316-117">String</span></span>|<span data-ttu-id="e7316-118">用户登录到的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="e7316-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="e7316-119">appId</span><span class="sxs-lookup"><span data-stu-id="e7316-119">appId</span></span>|<span data-ttu-id="e7316-120">String</span><span class="sxs-lookup"><span data-stu-id="e7316-120">String</span></span>|  <span data-ttu-id="e7316-121">用户签署的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="e7316-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="e7316-122">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="e7316-122">failedSignInCount</span></span>|<span data-ttu-id="e7316-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e7316-123">Int64</span></span>|<span data-ttu-id="e7316-124">应用程序发出的失败登录数。</span><span class="sxs-lookup"><span data-stu-id="e7316-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="e7316-125">successPercentage</span><span class="sxs-lookup"><span data-stu-id="e7316-125">successPercentage</span></span>|<span data-ttu-id="e7316-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e7316-126">Int32</span></span>|<span data-ttu-id="e7316-127">由应用程序成功登录所占的百分比。</span><span class="sxs-lookup"><span data-stu-id="e7316-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="e7316-128">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="e7316-128">successfulSignInCount</span></span>|<span data-ttu-id="e7316-129">Int64</span><span class="sxs-lookup"><span data-stu-id="e7316-129">Int64</span></span>|<span data-ttu-id="e7316-130">应用程序成功登录时所用的计数。</span><span class="sxs-lookup"><span data-stu-id="e7316-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7316-131">关系</span><span class="sxs-lookup"><span data-stu-id="e7316-131">Relationships</span></span>
<span data-ttu-id="e7316-132">无</span><span class="sxs-lookup"><span data-stu-id="e7316-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e7316-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7316-133">JSON representation</span></span>

<span data-ttu-id="e7316-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7316-134">The following is a JSON representation of the resource.</span></span>

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
