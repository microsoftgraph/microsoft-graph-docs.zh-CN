---
title: verifiedPublisher 资源类型
description: 表示已验证的应用程序发布者。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: d998b8bf3e5ab4ad253e31a96794e8e531e6803e
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921897"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="e6f40-103">verifiedPublisher 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6f40-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="e6f40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6f40-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6f40-105">表示已验证的 [应用程序](application.md)发布者。</span><span class="sxs-lookup"><span data-stu-id="e6f40-105">Represents the verified publisher of the [application](application.md).</span></span> <span data-ttu-id="e6f40-106">有关详细信息，请参阅 [Publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="e6f40-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="e6f40-107">已验证发布者是使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 设置的，只能使用 [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md)删除。</span><span class="sxs-lookup"><span data-stu-id="e6f40-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e6f40-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6f40-108">Properties</span></span>

| <span data-ttu-id="e6f40-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6f40-109">Property</span></span> | <span data-ttu-id="e6f40-110">类型</span><span class="sxs-lookup"><span data-stu-id="e6f40-110">Type</span></span> | <span data-ttu-id="e6f40-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6f40-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f40-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e6f40-112">displayName</span></span>|<span data-ttu-id="e6f40-113">字符串</span><span class="sxs-lookup"><span data-stu-id="e6f40-113">String</span></span>|<span data-ttu-id="e6f40-114">来自应用发布者的合作伙伴中心帐户的经验证的发布者名称。</span><span class="sxs-lookup"><span data-stu-id="e6f40-114">The verified publisher name from the app publisher's Partner Center account.</span></span>|
|<span data-ttu-id="e6f40-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="e6f40-115">verifiedPublisherId</span></span>|<span data-ttu-id="e6f40-116">字符串</span><span class="sxs-lookup"><span data-stu-id="e6f40-116">String</span></span>| <span data-ttu-id="e6f40-117">来自应用程序发布者的合作伙伴中心帐户的已验证发布者的 ID。</span><span class="sxs-lookup"><span data-stu-id="e6f40-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="e6f40-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6f40-118">addedDateTime</span></span>|<span data-ttu-id="e6f40-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="e6f40-119">DateTimeOffSet</span></span>| <span data-ttu-id="e6f40-120">首次添加或最近更新的已验证发布者时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="e6f40-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="e6f40-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6f40-121">JSON representation</span></span>
<span data-ttu-id="e6f40-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6f40-122">Here is a JSON representation of the resource.</span></span>

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


<!-- uuid: 7a355221-34dd-4579-9bdd-4c3e1909e1bb
2020-09-09 20:45:56 UTC -->
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
