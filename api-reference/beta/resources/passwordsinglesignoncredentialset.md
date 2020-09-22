---
title: passwordSingleSignOnCredentialSet 资源类型
description: 指示将用户或组的登录流完全定义为应用程序的一组凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 87aafa6e21171088f9b4b5eac318f6c9551e18ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998199"
---
# <a name="passwordsinglesignoncredentialset-resource-type"></a><span data-ttu-id="7b466-103">passwordSingleSignOnCredentialSet 资源类型</span><span class="sxs-lookup"><span data-stu-id="7b466-103">passwordSingleSignOnCredentialSet resource type</span></span>

<span data-ttu-id="7b466-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b466-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b466-105">指示将用户或组的登录流完全定义为应用程序的一组凭据。</span><span class="sxs-lookup"><span data-stu-id="7b466-105">Indicates a set of credentials that completely define a sign in flow for a user or group to an application.</span></span>

## <a name="properties"></a><span data-ttu-id="7b466-106">属性</span><span class="sxs-lookup"><span data-stu-id="7b466-106">Properties</span></span>

| <span data-ttu-id="7b466-107">属性</span><span class="sxs-lookup"><span data-stu-id="7b466-107">Property</span></span>     | <span data-ttu-id="7b466-108">类型</span><span class="sxs-lookup"><span data-stu-id="7b466-108">Type</span></span>        | <span data-ttu-id="7b466-109">说明</span><span class="sxs-lookup"><span data-stu-id="7b466-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b466-110">凭据</span><span class="sxs-lookup"><span data-stu-id="7b466-110">credentials</span></span>|<span data-ttu-id="7b466-111">[凭据](credential.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7b466-111">[credential](credential.md) collection</span></span>|<span data-ttu-id="7b466-112">定义完整的登录流的 credential 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7b466-112">A list of credential objects that define the complete sign in flow.</span></span>|
|<span data-ttu-id="7b466-113">id</span><span class="sxs-lookup"><span data-stu-id="7b466-113">id</span></span>|<span data-ttu-id="7b466-114">String</span><span class="sxs-lookup"><span data-stu-id="7b466-114">String</span></span>|<span data-ttu-id="7b466-115">此凭据集所属的用户或组的 ID。</span><span class="sxs-lookup"><span data-stu-id="7b466-115">The ID of the user or group this credential set belongs to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b466-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7b466-116">JSON representation</span></span>

<span data-ttu-id="7b466-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7b466-117">The following is a JSON representation of the resource.</span></span>

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


