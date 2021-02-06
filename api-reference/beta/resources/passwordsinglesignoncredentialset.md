---
title: passwordSingleSignOnCredentialSet 资源类型
description: 指示完全定义用户或组到应用程序的登录流的凭据集。
localization_priority: Normal
author: bharathramh92
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 95526942bcedfc20d983a8873699af6902482b2c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130874"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="f14a5-103">passwordSingleSignOnCredentialSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="f14a5-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="f14a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f14a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f14a5-105">指示完全定义用户或组到应用程序的登录流的凭据集。</span><span class="sxs-lookup"><span data-stu-id="f14a5-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="f14a5-106">属性</span><span class="sxs-lookup"><span data-stu-id="f14a5-106">Properties</span></span>

| <span data-ttu-id="f14a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="f14a5-107">Property</span></span>     | <span data-ttu-id="f14a5-108">类型</span><span class="sxs-lookup"><span data-stu-id="f14a5-108">Type</span></span>        | <span data-ttu-id="f14a5-109">说明</span><span class="sxs-lookup"><span data-stu-id="f14a5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f14a5-110">credentials</span><span class="sxs-lookup"><span data-stu-id="f14a5-110">credentials</span></span>|<span data-ttu-id="f14a5-111">[credential](credential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f14a5-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="f14a5-112">定义完整登录流的凭据对象列表。</span><span class="sxs-lookup"><span data-stu-id="f14a5-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="f14a5-113">id</span><span class="sxs-lookup"><span data-stu-id="f14a5-113">id</span></span>|<span data-ttu-id="f14a5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f14a5-114">String</span></span>|<span data-ttu-id="f14a5-115">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="f14a5-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f14a5-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f14a5-116">JSON representation</span></span>

<span data-ttu-id="f14a5-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f14a5-117">The following is a JSON representation of the resource.</span></span>

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


