---
title: verifiedPublisher 资源类型
description: 表示已验证的应用程序发布者。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jesakowi
ms.openlocfilehash: 0d704b42c83a853d094406c0ba62010da30ce142
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471553"
---
# <a name="verifiedpublisher-resource-type"></a><span data-ttu-id="c174a-103">verifiedPublisher 资源类型</span><span class="sxs-lookup"><span data-stu-id="c174a-103">verifiedPublisher resource type</span></span>

<span data-ttu-id="c174a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c174a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c174a-105">表示已验证的 [应用程序](application.md)发布者。</span><span class="sxs-lookup"><span data-stu-id="c174a-105">Represents a verified publisher of an [application](application.md).</span></span> <span data-ttu-id="c174a-106">有关详细信息，请参阅 [Publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="c174a-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span> <span data-ttu-id="c174a-107">已验证发布者是使用 [setVerifiedPublisher](../api/application-setverifiedpublisher.md) 设置的，只能使用 [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md)删除。</span><span class="sxs-lookup"><span data-stu-id="c174a-107">Verified publishers are set using [setVerifiedPublisher](../api/application-setverifiedpublisher.md) and can only be removed using [unsetVerifiedPublisher](../api/application-unsetverifiedpublisher.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c174a-108">属性</span><span class="sxs-lookup"><span data-stu-id="c174a-108">Properties</span></span>

| <span data-ttu-id="c174a-109">属性</span><span class="sxs-lookup"><span data-stu-id="c174a-109">Property</span></span> | <span data-ttu-id="c174a-110">类型</span><span class="sxs-lookup"><span data-stu-id="c174a-110">Type</span></span> | <span data-ttu-id="c174a-111">说明</span><span class="sxs-lookup"><span data-stu-id="c174a-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c174a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c174a-112">displayName</span></span>|<span data-ttu-id="c174a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="c174a-113">String</span></span>|<span data-ttu-id="c174a-114">来自应用发布者的 Microsoft 合作伙伴网络的经验证的发布者名称 (MPN) 帐户。</span><span class="sxs-lookup"><span data-stu-id="c174a-114">The verified publisher name from the app publisher's Microsoft Partner Network (MPN) account.</span></span>|
|<span data-ttu-id="c174a-115">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="c174a-115">verifiedPublisherId</span></span>|<span data-ttu-id="c174a-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c174a-116">String</span></span>| <span data-ttu-id="c174a-117">来自应用程序发布者的合作伙伴中心帐户的已验证发布者的 ID。</span><span class="sxs-lookup"><span data-stu-id="c174a-117">The ID of the verified publisher from the app publisher's Partner Center account.</span></span> |
|<span data-ttu-id="c174a-118">addedDateTime</span><span class="sxs-lookup"><span data-stu-id="c174a-118">addedDateTime</span></span>|<span data-ttu-id="c174a-119">DateTimeOffSet</span><span class="sxs-lookup"><span data-stu-id="c174a-119">DateTimeOffSet</span></span>| <span data-ttu-id="c174a-120">首次添加或最近更新的已验证发布者时的时间戳。</span><span class="sxs-lookup"><span data-stu-id="c174a-120">The timestamp when the verified publisher was first added or most recently updated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c174a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c174a-121">JSON representation</span></span>
<span data-ttu-id="c174a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c174a-122">Here is a JSON representation of the resource.</span></span>

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
