---
title: credential 资源类型
description: 指示用于登录应用程序的单个凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3b23249d7c0b898344113c5bcfe950c207891250
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658882"
---
# <a name="credential-resource-type"></a><span data-ttu-id="fda95-103">credential 资源类型</span><span class="sxs-lookup"><span data-stu-id="fda95-103">credential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fda95-104">指示用于登录应用程序的单个凭据。</span><span class="sxs-lookup"><span data-stu-id="fda95-104">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="fda95-105">例如，username 是一个凭据，即 "密码" 是另一个凭据。</span><span class="sxs-lookup"><span data-stu-id="fda95-105">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="fda95-106">属性</span><span class="sxs-lookup"><span data-stu-id="fda95-106">Properties</span></span>

| <span data-ttu-id="fda95-107">属性</span><span class="sxs-lookup"><span data-stu-id="fda95-107">Property</span></span>     | <span data-ttu-id="fda95-108">类型</span><span class="sxs-lookup"><span data-stu-id="fda95-108">Type</span></span>        | <span data-ttu-id="fda95-109">说明</span><span class="sxs-lookup"><span data-stu-id="fda95-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fda95-110">fieldId</span><span class="sxs-lookup"><span data-stu-id="fda95-110">fieldId</span></span>|<span data-ttu-id="fda95-111">字符串</span><span class="sxs-lookup"><span data-stu-id="fda95-111">String</span></span>|<span data-ttu-id="fda95-112">此凭据的字段名称。</span><span class="sxs-lookup"><span data-stu-id="fda95-112">The name of the field for this credential.</span></span> <span data-ttu-id="fda95-113">例如，username、password 或 phoneNumber。</span><span class="sxs-lookup"><span data-stu-id="fda95-113">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="fda95-114">这是由应用程序定义的。</span><span class="sxs-lookup"><span data-stu-id="fda95-114">This is defined by the application.</span></span> <span data-ttu-id="fda95-115">必须与 singleSignOnSettings/password 对象上的 html 字段中的内容相匹配。</span><span class="sxs-lookup"><span data-stu-id="fda95-115">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="fda95-116">type</span><span class="sxs-lookup"><span data-stu-id="fda95-116">type</span></span>|<span data-ttu-id="fda95-117">字符串</span><span class="sxs-lookup"><span data-stu-id="fda95-117">String</span></span>|<span data-ttu-id="fda95-118">此凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="fda95-118">The type for this credential.</span></span> <span data-ttu-id="fda95-119">有效值： username、password 或其他值。</span><span class="sxs-lookup"><span data-stu-id="fda95-119">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="fda95-120">value</span><span class="sxs-lookup"><span data-stu-id="fda95-120">value</span></span>|<span data-ttu-id="fda95-121">String</span><span class="sxs-lookup"><span data-stu-id="fda95-121">String</span></span>|<span data-ttu-id="fda95-122">此凭据的值。</span><span class="sxs-lookup"><span data-stu-id="fda95-122">The value for this credential.</span></span> <span data-ttu-id="fda95-123">例如，mysuperhiddenpassword。</span><span class="sxs-lookup"><span data-stu-id="fda95-123">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="fda95-124">注意：密码的值是只写的，该值永远不能读回。</span><span class="sxs-lookup"><span data-stu-id="fda95-124">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fda95-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fda95-125">JSON representation</span></span>

<span data-ttu-id="fda95-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fda95-126">The following is a JSON representation of the resource.</span></span>

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
