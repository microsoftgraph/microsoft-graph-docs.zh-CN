---
title: 设置资源类型
description: 用户使用分析 API 时所需的当前设置。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 822ac02be4f3dc5d507aa5d9dbbb2fa22b194b64
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033533"
---
# <a name="settings-resource-type"></a><span data-ttu-id="acf19-103">设置资源类型</span><span class="sxs-lookup"><span data-stu-id="acf19-103">settings resource type</span></span>

<span data-ttu-id="acf19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acf19-105">表示用户使用分析 API 时所需的当前设置。</span><span class="sxs-lookup"><span data-stu-id="acf19-105">Represents the current required settings for a user to use the analytics API.</span></span>

<span data-ttu-id="acf19-106">若要使分析 API 返回用户的结果，他们必须拥有为 Microsoft Graph 启用的云托管邮箱，具有有效的 MyAnalytics 许可证，并选择使用 MyAnalytics。</span><span class="sxs-lookup"><span data-stu-id="acf19-106">For the analytics API to return results for users, they must have a cloud-hosted mailbox that’s enabled for Microsoft Graph, have a valid MyAnalytics license, and be opted in to using MyAnalytics.</span></span>

## <a name="methods"></a><span data-ttu-id="acf19-107">方法</span><span class="sxs-lookup"><span data-stu-id="acf19-107">Methods</span></span>

| <span data-ttu-id="acf19-108">方法</span><span class="sxs-lookup"><span data-stu-id="acf19-108">Method</span></span>       | <span data-ttu-id="acf19-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="acf19-109">Return Type</span></span> | <span data-ttu-id="acf19-110">说明</span><span class="sxs-lookup"><span data-stu-id="acf19-110">Description</span></span> |
|:-------------|:------------|:------------|
[<span data-ttu-id="acf19-111">获取设置</span><span class="sxs-lookup"><span data-stu-id="acf19-111">Get settings</span></span>](../api/useranalytics-get-settings.md) | [<span data-ttu-id="acf19-112">设置</span><span class="sxs-lookup"><span data-stu-id="acf19-112">settings</span></span>](settings.md) | <span data-ttu-id="acf19-113">获取用户的以下属性设置。</span><span class="sxs-lookup"><span data-stu-id="acf19-113">Get the following property settings for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="acf19-114">属性</span><span class="sxs-lookup"><span data-stu-id="acf19-114">Properties</span></span>

| <span data-ttu-id="acf19-115">属性</span><span class="sxs-lookup"><span data-stu-id="acf19-115">Property</span></span>     | <span data-ttu-id="acf19-116">类型</span><span class="sxs-lookup"><span data-stu-id="acf19-116">Type</span></span>        | <span data-ttu-id="acf19-117">说明</span><span class="sxs-lookup"><span data-stu-id="acf19-117">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="acf19-118">hasGraphMailbox</span><span class="sxs-lookup"><span data-stu-id="acf19-118">hasGraphMailbox</span></span>|<span data-ttu-id="acf19-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf19-119">Boolean</span></span>|<span data-ttu-id="acf19-120">指定用户的主邮箱是否托管在云中，是否已为 Microsoft Graph 启用。</span><span class="sxs-lookup"><span data-stu-id="acf19-120">Specifies if the user's primary mailbox is hosted in the cloud and is enabled for Microsoft Graph.</span></span>|
|<span data-ttu-id="acf19-121">hasLicense</span><span class="sxs-lookup"><span data-stu-id="acf19-121">hasLicense</span></span>|<span data-ttu-id="acf19-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf19-122">Boolean</span></span>|<span data-ttu-id="acf19-123">指定是否为用户分配了 MyAnalytics 许可证。</span><span class="sxs-lookup"><span data-stu-id="acf19-123">Specifies if the user has a MyAnalytics license assigned.</span></span>|
|<span data-ttu-id="acf19-124">hasOptedOut</span><span class="sxs-lookup"><span data-stu-id="acf19-124">hasOptedOut</span></span>|<span data-ttu-id="acf19-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="acf19-125">Boolean</span></span>|<span data-ttu-id="acf19-126">指定用户是否选择了 "MyAnalytics"。</span><span class="sxs-lookup"><span data-stu-id="acf19-126">Specifies if the user opted out of MyAnalytics.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="acf19-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="acf19-127">JSON representation</span></span>

<span data-ttu-id="acf19-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="acf19-128">The following is a JSON representation of the resource.</span></span>

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

