---
title: applicationSignInDetailedSummary 资源类型
description: 表示应用程序登录摘要。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0329aec304602151a23ff389bc041247f9fb65b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339038"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="29365-103">applicationSignInSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="29365-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29365-104">表示应用程序登录摘要。</span><span class="sxs-lookup"><span data-stu-id="29365-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="29365-105">方法</span><span class="sxs-lookup"><span data-stu-id="29365-105">Methods</span></span>

| <span data-ttu-id="29365-106">方法</span><span class="sxs-lookup"><span data-stu-id="29365-106">Method</span></span>       | <span data-ttu-id="29365-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="29365-107">Return Type</span></span> | <span data-ttu-id="29365-108">说明</span><span class="sxs-lookup"><span data-stu-id="29365-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="29365-109">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="29365-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="29365-110">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="29365-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="29365-111">读取**applicationSignInSummary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29365-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29365-112">属性</span><span class="sxs-lookup"><span data-stu-id="29365-112">Properties</span></span>
| <span data-ttu-id="29365-113">属性</span><span class="sxs-lookup"><span data-stu-id="29365-113">Property</span></span>     | <span data-ttu-id="29365-114">类型</span><span class="sxs-lookup"><span data-stu-id="29365-114">Type</span></span>        | <span data-ttu-id="29365-115">说明</span><span class="sxs-lookup"><span data-stu-id="29365-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29365-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="29365-116">appDisplayName</span></span>|<span data-ttu-id="29365-117">String</span><span class="sxs-lookup"><span data-stu-id="29365-117">String</span></span>|<span data-ttu-id="29365-118">用户登录到的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="29365-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="29365-119">appId</span><span class="sxs-lookup"><span data-stu-id="29365-119">appId</span></span>|<span data-ttu-id="29365-120">String</span><span class="sxs-lookup"><span data-stu-id="29365-120">String</span></span>|  <span data-ttu-id="29365-121">用户签署的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="29365-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="29365-122">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="29365-122">failedSignInCount</span></span>|<span data-ttu-id="29365-123">Int64</span><span class="sxs-lookup"><span data-stu-id="29365-123">Int64</span></span>|<span data-ttu-id="29365-124">应用程序发出的失败登录数。</span><span class="sxs-lookup"><span data-stu-id="29365-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="29365-125">successPercentage</span><span class="sxs-lookup"><span data-stu-id="29365-125">successPercentage</span></span>|<span data-ttu-id="29365-126">Int32</span><span class="sxs-lookup"><span data-stu-id="29365-126">Int32</span></span>|<span data-ttu-id="29365-127">由应用程序成功登录所占的百分比。</span><span class="sxs-lookup"><span data-stu-id="29365-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="29365-128">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="29365-128">successfulSignInCount</span></span>|<span data-ttu-id="29365-129">Int64</span><span class="sxs-lookup"><span data-stu-id="29365-129">Int64</span></span>|<span data-ttu-id="29365-130">应用程序成功登录时所用的计数。</span><span class="sxs-lookup"><span data-stu-id="29365-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29365-131">关系</span><span class="sxs-lookup"><span data-stu-id="29365-131">Relationships</span></span>
<span data-ttu-id="29365-132">无</span><span class="sxs-lookup"><span data-stu-id="29365-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="29365-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29365-133">JSON representation</span></span>

<span data-ttu-id="29365-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29365-134">The following is a JSON representation of the resource.</span></span>

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
