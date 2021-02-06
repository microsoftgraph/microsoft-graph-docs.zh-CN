---
title: verifiedPublisher 资源类型
description: 表示应用程序的已验证发布者。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 5acc66bd72c65b25d8301c4870fa5ff0f98a0d73
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135623"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="043e4-103">verifiedPublisher 资源类型</span><span class="sxs-lookup"><span data-stu-id="043e4-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="043e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="043e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="043e4-105">表示应用程序的已验证 [发布者](application.md)。</span><span class="sxs-lookup"><span data-stu-id="043e4-105">Represents a verified publisher of an [application](application.md).</span></span> <span data-ttu-id="043e4-106">有关详细信息，请参阅 [发布者验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="043e4-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="043e4-107">已验证发布者是使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 设置的，并且只能使用 [unsetVerifiedPublisher 删除](../api/application-unsetverifiedpublisher.md)。</span><span class="sxs-lookup"><span data-stu-id="043e4-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="043e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="043e4-108">Properties</span></span>

| <span data-ttu-id="043e4-109">属性</span><span class="sxs-lookup"><span data-stu-id="043e4-109">Property</span></span> | <span data-ttu-id="043e4-110">类型</span><span class="sxs-lookup"><span data-stu-id="043e4-110">Type</span></span> | <span data-ttu-id="043e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="043e4-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="043e4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="043e4-112">displayName</span></span>|<span data-ttu-id="043e4-113">字符串</span><span class="sxs-lookup"><span data-stu-id="043e4-113">String</span></span>|<span data-ttu-id="043e4-114">来自应用发布者的 Microsoft 合作伙伴网络的验证发布者名称 (MPN) 帐户。</span><span class="sxs-lookup"><span data-stu-id="043e4-114">The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.</span></span>|
|<span data-ttu-id="043e4-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="043e4-115">verifiedPublisherId</span></span>|<span data-ttu-id="043e4-116">字符串</span><span class="sxs-lookup"><span data-stu-id="043e4-116">String</span></span>| <span data-ttu-id="043e4-117">应用发布者的合作伙伴中心帐户中经过验证的发布者的 ID。</span><span class="sxs-lookup"><span data-stu-id="043e4-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="043e4-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="043e4-118">addedDateTime</span></span>|<span data-ttu-id="043e4-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="043e4-119">DateTimeOffSet</span></span>| <span data-ttu-id="043e4-120">首次添加或最近更新已验证发布者的时间戳。</span><span class="sxs-lookup"><span data-stu-id="043e4-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="043e4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="043e4-121">JSON representation</span></span>
<span data-ttu-id="043e4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="043e4-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedPublisher"
}-->

```json
{
  "displayName": "String",
  "verifiedPublisherId": "String",
  "addedDateTime": "DateTimeOffSet"
}

```


<!-- uuid: e9aa37e1-f0b7-4201-a6b2-d26ce091dff6
2020-09-09 20:42:32 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedPublisher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
