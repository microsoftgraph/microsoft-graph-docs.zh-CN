---
title: verifiedPublisher 资源类型
description: 表示应用程序的已验证发布者。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: jesakowi
ms.openlocfilehash: 0c7d500a4fd032704f36953c8bf18efe6fa0f68d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129677"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="f67a6-103">verifiedPublisher 资源类型</span><span class="sxs-lookup"><span data-stu-id="f67a6-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="f67a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f67a6-105">表示应用程序的已验证 [发布者](application.md)。</span><span class="sxs-lookup"><span data-stu-id="f67a6-105">Represents the verified publisher of the [application](application.md).</span></span> <span data-ttu-id="f67a6-106">有关详细信息，请参阅 [发布者验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="f67a6-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="f67a6-107">已验证发布者是使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 设置的，并且只能使用 [unsetVerifiedPublisher 删除](../api/application-unsetverifiedpublisher.md)。</span><span class="sxs-lookup"><span data-stu-id="f67a6-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f67a6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f67a6-108">Properties</span></span>

| <span data-ttu-id="f67a6-109">属性</span><span class="sxs-lookup"><span data-stu-id="f67a6-109">Property</span></span> | <span data-ttu-id="f67a6-110">类型</span><span class="sxs-lookup"><span data-stu-id="f67a6-110">Type</span></span> | <span data-ttu-id="f67a6-111">说明</span><span class="sxs-lookup"><span data-stu-id="f67a6-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f67a6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f67a6-112">displayName</span></span>|<span data-ttu-id="f67a6-113">String</span><span class="sxs-lookup"><span data-stu-id="f67a6-113">String</span></span>|<span data-ttu-id="f67a6-114">应用发布者的合作伙伴中心帐户中的已验证发布者名称。</span><span class="sxs-lookup"><span data-stu-id="f67a6-114">The verified publisher name from the app publisher's Partner Center account.</span></span>|
|<span data-ttu-id="f67a6-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="f67a6-115">verifiedPublisherId</span></span>|<span data-ttu-id="f67a6-116">String</span><span class="sxs-lookup"><span data-stu-id="f67a6-116">String</span></span>| <span data-ttu-id="f67a6-117">应用发布者的合作伙伴中心帐户中经过验证的发布者的 ID。</span><span class="sxs-lookup"><span data-stu-id="f67a6-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="f67a6-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="f67a6-118">addedDateTime</span></span>|<span data-ttu-id="f67a6-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="f67a6-119">DateTimeOffSet</span></span>| <span data-ttu-id="f67a6-120">首次添加或最近更新已验证发布者的时间戳。</span><span class="sxs-lookup"><span data-stu-id="f67a6-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f67a6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f67a6-121">JSON representation</span></span>
<span data-ttu-id="f67a6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f67a6-122">Here is a JSON representation of the resource.</span></span>

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
