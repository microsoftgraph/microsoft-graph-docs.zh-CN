---
title: credential 资源类型
description: 指示用于登录应用程序的单个凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a281e39850ea18ee3bcbe0d83c5df3b41d0ccd31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016686"
---
# <a name="credential-resource-type"></a><span data-ttu-id="b4324-103">credential 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4324-103">credential resource type</span></span>

<span data-ttu-id="b4324-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4324-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4324-105">指示用于登录应用程序的单个凭据。</span><span class="sxs-lookup"><span data-stu-id="b4324-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="b4324-106">例如，username 是一个凭据，即 "密码" 是另一个凭据。</span><span class="sxs-lookup"><span data-stu-id="b4324-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="b4324-107">属性</span><span class="sxs-lookup"><span data-stu-id="b4324-107">Properties</span></span>

| <span data-ttu-id="b4324-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4324-108">Property</span></span>     | <span data-ttu-id="b4324-109">类型</span><span class="sxs-lookup"><span data-stu-id="b4324-109">Type</span></span>        | <span data-ttu-id="b4324-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4324-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b4324-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="b4324-111">fieldId</span></span>|<span data-ttu-id="b4324-112">String</span><span class="sxs-lookup"><span data-stu-id="b4324-112">String</span></span>|<span data-ttu-id="b4324-113">此凭据的字段名称。</span><span class="sxs-lookup"><span data-stu-id="b4324-113">The name of the field for this credential.</span></span> <span data-ttu-id="b4324-114">例如，username、password 或 phoneNumber。</span><span class="sxs-lookup"><span data-stu-id="b4324-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="b4324-115">这是由应用程序定义的。</span><span class="sxs-lookup"><span data-stu-id="b4324-115">This is defined by the application.</span></span> <span data-ttu-id="b4324-116">必须与 singleSignOnSettings/password 对象上的 html 字段中的内容相匹配。</span><span class="sxs-lookup"><span data-stu-id="b4324-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="b4324-117">type</span><span class="sxs-lookup"><span data-stu-id="b4324-117">type</span></span>|<span data-ttu-id="b4324-118">String</span><span class="sxs-lookup"><span data-stu-id="b4324-118">String</span></span>|<span data-ttu-id="b4324-119">此凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="b4324-119">The type for this credential.</span></span> <span data-ttu-id="b4324-120">有效值： username、password 或其他值。</span><span class="sxs-lookup"><span data-stu-id="b4324-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="b4324-121">value</span><span class="sxs-lookup"><span data-stu-id="b4324-121">value</span></span>|<span data-ttu-id="b4324-122">String</span><span class="sxs-lookup"><span data-stu-id="b4324-122">String</span></span>|<span data-ttu-id="b4324-123">此凭据的值。</span><span class="sxs-lookup"><span data-stu-id="b4324-123">The value for this credential.</span></span> <span data-ttu-id="b4324-124">例如，mysuperhiddenpassword。</span><span class="sxs-lookup"><span data-stu-id="b4324-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="b4324-125">注意：密码的值是只写的，该值永远不能读回。</span><span class="sxs-lookup"><span data-stu-id="b4324-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4324-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4324-126">JSON representation</span></span>

<span data-ttu-id="b4324-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4324-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.credential",
  "baseType": null
}-->

```json
{
  "fieldId": "param_username",
  "value": "myusername",
  "type": "username"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "credential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


