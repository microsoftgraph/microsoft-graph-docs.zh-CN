---
title: 设置资源类型
description: 用户使用分析 API 时所需的当前设置。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a7d534aecf6e7ffa427ea175ae06e2b1820435b2
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450728"
---
# <a name="settings-resource-type"></a><span data-ttu-id="d0ed8-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="d0ed8-103">settings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0ed8-104">表示用户使用分析 API 时所需的当前设置。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-104">Represents the current required settings for a user to use the analytics API.</span></span>

<span data-ttu-id="d0ed8-105">若要使分析 API 返回用户的结果, 他们必须拥有为 Microsoft Graph 启用的云托管邮箱, 具有有效的 MyAnalytics 许可证, 并选择使用 MyAnalytics。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-105">For the analytics API to return results for users, they must have a cloud-hosted mailbox that’s enabled for Microsoft Graph, have a valid MyAnalytics license, and be opted in to using MyAnalytics.</span></span>

## <a name="methods"></a><span data-ttu-id="d0ed8-106">方法</span><span class="sxs-lookup"><span data-stu-id="d0ed8-106">Methods</span></span>

| <span data-ttu-id="d0ed8-107">方法</span><span class="sxs-lookup"><span data-stu-id="d0ed8-107">Method</span></span>       | <span data-ttu-id="d0ed8-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0ed8-108">Return Type</span></span> | <span data-ttu-id="d0ed8-109">说明</span><span class="sxs-lookup"><span data-stu-id="d0ed8-109">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="d0ed8-110">获取设置</span><span class="sxs-lookup"><span data-stu-id="d0ed8-110">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="d0ed8-111">settings</span><span class="sxs-lookup"><span data-stu-id="d0ed8-111">settings</span></span>](settings.md) | <span data-ttu-id="d0ed8-112">获取用户的以下属性设置。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-112">Get the following property settings for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="d0ed8-113">属性</span><span class="sxs-lookup"><span data-stu-id="d0ed8-113">Properties</span></span>

| <span data-ttu-id="d0ed8-114">属性</span><span class="sxs-lookup"><span data-stu-id="d0ed8-114">Property</span></span>     | <span data-ttu-id="d0ed8-115">类型</span><span class="sxs-lookup"><span data-stu-id="d0ed8-115">Type</span></span>        | <span data-ttu-id="d0ed8-116">说明</span><span class="sxs-lookup"><span data-stu-id="d0ed8-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0ed8-117">hasGraphMailbox</span><span class="sxs-lookup"><span data-stu-id="d0ed8-117">hasGraphMailbox</span></span>|<span data-ttu-id="d0ed8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0ed8-118">Boolean</span></span>|<span data-ttu-id="d0ed8-119">指定用户的主邮箱是否托管在云中, 是否已为 Microsoft Graph 启用。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-119">Specifies if the user's primary mailbox is hosted in the cloud and is enabled for Microsoft Graph.</span></span>|
|<span data-ttu-id="d0ed8-120">hasLicense</span><span class="sxs-lookup"><span data-stu-id="d0ed8-120">hasLicense</span></span>|<span data-ttu-id="d0ed8-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0ed8-121">Boolean</span></span>|<span data-ttu-id="d0ed8-122">指定是否为用户分配了 MyAnalytics 许可证。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-122">Specifies if the user has a MyAnalytics license assigned.</span></span>|
|<span data-ttu-id="d0ed8-123">hasOptedOut</span><span class="sxs-lookup"><span data-stu-id="d0ed8-123">hasOptedOut</span></span>|<span data-ttu-id="d0ed8-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0ed8-124">Boolean</span></span>|<span data-ttu-id="d0ed8-125">指定用户是否选择了 "MyAnalytics"。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-125">Specifies if the user opted out of MyAnalytics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0ed8-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0ed8-126">JSON representation</span></span>

<span data-ttu-id="d0ed8-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0ed8-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settings",
  "baseType": null
}-->

```json
{
  "hasGraphMailbox": true,
  "hasLicense": true,
  "hasOptedOut": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->