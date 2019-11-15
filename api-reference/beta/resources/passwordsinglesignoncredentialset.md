---
title: passwordSingleSignOnCredentialSet 资源类型
description: 指示将用户或组的登录流完全定义为应用程序的一组凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6293c6a2fbdffd124a8e011bd00a22c30efa77e5
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658791"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="7d3ff-103">passwordSingleSignOnCredentialSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d3ff-103">passwordSingleSignOnCredentialSet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d3ff-104">指示将用户或组的登录流完全定义为应用程序的一组凭据。</span><span class="sxs-lookup"><span data-stu-id="7d3ff-104">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="7d3ff-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d3ff-105">Properties</span></span>

| <span data-ttu-id="7d3ff-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d3ff-106">Property</span></span>     | <span data-ttu-id="7d3ff-107">类型</span><span class="sxs-lookup"><span data-stu-id="7d3ff-107">Type</span></span>        | <span data-ttu-id="7d3ff-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d3ff-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7d3ff-109">凭据</span><span class="sxs-lookup"><span data-stu-id="7d3ff-109">credentials</span></span>|<span data-ttu-id="7d3ff-110">[凭据](credential.md)集合</span><span class="sxs-lookup"><span data-stu-id="7d3ff-110">[credential](credential.md) collection</span></span>|<span data-ttu-id="7d3ff-111">定义完整的登录流的 credential 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7d3ff-111">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="7d3ff-112">id</span><span class="sxs-lookup"><span data-stu-id="7d3ff-112">id</span></span>|<span data-ttu-id="7d3ff-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7d3ff-113">String</span></span>|<span data-ttu-id="7d3ff-114">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="7d3ff-114">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7d3ff-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d3ff-115">JSON representation</span></span>

<span data-ttu-id="7d3ff-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d3ff-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnCredentialSet",
  "baseType": null
}-->

```json
{
  "credentials": [{"@odata.type": "microsoft.graph.credential"}],
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnCredentialSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
