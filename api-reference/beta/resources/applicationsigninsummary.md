---
title: applicationSignInDetailedSummary 资源类型
description: 表示应用程序登录摘要。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0329aec304602151a23ff389bc041247f9fb65b7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32655385"
---
# <a name="applicationsigninsummary-resource-type"></a><span data-ttu-id="001a4-103">applicationSignInSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="001a4-103">applicationSignInSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="001a4-104">表示应用程序登录摘要。</span><span class="sxs-lookup"><span data-stu-id="001a4-104">Represents an application sign-in summary.</span></span>

## <a name="methods"></a><span data-ttu-id="001a4-105">方法</span><span class="sxs-lookup"><span data-stu-id="001a4-105">Methods</span></span>

| <span data-ttu-id="001a4-106">方法</span><span class="sxs-lookup"><span data-stu-id="001a4-106">Method</span></span>       | <span data-ttu-id="001a4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="001a4-107">Return Type</span></span> | <span data-ttu-id="001a4-108">说明</span><span class="sxs-lookup"><span data-stu-id="001a4-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="001a4-109">获取 applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="001a4-109">Get applicationSignInSummary</span></span>](../api/applicationsigninsummary-get.md) | [<span data-ttu-id="001a4-110">applicationSignInSummary</span><span class="sxs-lookup"><span data-stu-id="001a4-110">applicationSignInSummary</span></span>](applicationsigninsummary.md) | <span data-ttu-id="001a4-111">读取**applicationSignInSummary**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="001a4-111">Read the properties and relationships of an **applicationSignInSummary** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="001a4-112">属性</span><span class="sxs-lookup"><span data-stu-id="001a4-112">Properties</span></span>
| <span data-ttu-id="001a4-113">属性</span><span class="sxs-lookup"><span data-stu-id="001a4-113">Property</span></span>     | <span data-ttu-id="001a4-114">类型</span><span class="sxs-lookup"><span data-stu-id="001a4-114">Type</span></span>        | <span data-ttu-id="001a4-115">说明</span><span class="sxs-lookup"><span data-stu-id="001a4-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="001a4-116">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="001a4-116">appDisplayName</span></span>|<span data-ttu-id="001a4-117">String</span><span class="sxs-lookup"><span data-stu-id="001a4-117">String</span></span>|<span data-ttu-id="001a4-118">用户登录到的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="001a4-118">Name of the application that the user signed in to.</span></span>|
|<span data-ttu-id="001a4-119">appId</span><span class="sxs-lookup"><span data-stu-id="001a4-119">appId</span></span>|<span data-ttu-id="001a4-120">String</span><span class="sxs-lookup"><span data-stu-id="001a4-120">String</span></span>|  <span data-ttu-id="001a4-121">用户签署的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="001a4-121">ID of the application that the user signed i nto.</span></span>|
|<span data-ttu-id="001a4-122">failedSignInCount</span><span class="sxs-lookup"><span data-stu-id="001a4-122">failedSignInCount</span></span>|<span data-ttu-id="001a4-123">Int64</span><span class="sxs-lookup"><span data-stu-id="001a4-123">Int64</span></span>|<span data-ttu-id="001a4-124">应用程序发出的失败登录数。</span><span class="sxs-lookup"><span data-stu-id="001a4-124">Count of failed sign-ins made by the application.</span></span>|
|<span data-ttu-id="001a4-125">successPercentage</span><span class="sxs-lookup"><span data-stu-id="001a4-125">successPercentage</span></span>|<span data-ttu-id="001a4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="001a4-126">Int32</span></span>|<span data-ttu-id="001a4-127">由应用程序成功登录所占的百分比。</span><span class="sxs-lookup"><span data-stu-id="001a4-127">Percentage of successful sign-ins made by the application.</span></span>|
|<span data-ttu-id="001a4-128">successfulSignInCount</span><span class="sxs-lookup"><span data-stu-id="001a4-128">successfulSignInCount</span></span>|<span data-ttu-id="001a4-129">Int64</span><span class="sxs-lookup"><span data-stu-id="001a4-129">Int64</span></span>|<span data-ttu-id="001a4-130">应用程序成功登录时所用的计数。</span><span class="sxs-lookup"><span data-stu-id="001a4-130">Count of successful sign-ins made by the application.</span></span>|

## <a name="relationships"></a><span data-ttu-id="001a4-131">关系</span><span class="sxs-lookup"><span data-stu-id="001a4-131">Relationships</span></span>
<span data-ttu-id="001a4-132">无</span><span class="sxs-lookup"><span data-stu-id="001a4-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="001a4-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="001a4-133">JSON representation</span></span>

<span data-ttu-id="001a4-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="001a4-134">The following is a JSON representation of the resource.</span></span>

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
