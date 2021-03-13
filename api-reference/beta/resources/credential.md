---
title: 凭据资源类型
description: 指示用于登录应用程序的单个凭据。
localization_priority: Normal
author: bharathramh92
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0521f766a7a0da482cf67628c3816935ee9270b8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761679"
---
# <a name="credential-resource-type"></a><span data-ttu-id="0e937-103">凭据资源类型</span><span class="sxs-lookup"><span data-stu-id="0e937-103">credential resource type</span></span>

<span data-ttu-id="0e937-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e937-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e937-105">指示用于登录应用程序的单个凭据。</span><span class="sxs-lookup"><span data-stu-id="0e937-105">Indicates a single credential used for sign-in to an application.</span></span> <span data-ttu-id="0e937-106">例如，username 是一个凭据，password 是另一个凭据。</span><span class="sxs-lookup"><span data-stu-id="0e937-106">For example, username is one credential, password is another credential.</span></span>

## <a name="properties"></a><span data-ttu-id="0e937-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e937-107">Properties</span></span>

| <span data-ttu-id="0e937-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e937-108">Property</span></span>     | <span data-ttu-id="0e937-109">类型</span><span class="sxs-lookup"><span data-stu-id="0e937-109">Type</span></span>        | <span data-ttu-id="0e937-110">说明</span><span class="sxs-lookup"><span data-stu-id="0e937-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e937-111">fieldId</span><span class="sxs-lookup"><span data-stu-id="0e937-111">fieldId</span></span>|<span data-ttu-id="0e937-112">String</span><span class="sxs-lookup"><span data-stu-id="0e937-112">String</span></span>|<span data-ttu-id="0e937-113">此凭据的字段名称。</span><span class="sxs-lookup"><span data-stu-id="0e937-113">The name of the field for this credential.</span></span> <span data-ttu-id="0e937-114">例如用户名或密码或 phoneNumber。</span><span class="sxs-lookup"><span data-stu-id="0e937-114">e.g, username or password or phoneNumber.</span></span> <span data-ttu-id="0e937-115">这由应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="0e937-115">This is defined by the application.</span></span> <span data-ttu-id="0e937-116">必须与 singleSignOnSettings/password 对象上的 html 字段中的项匹配。</span><span class="sxs-lookup"><span data-stu-id="0e937-116">Must match what is in the html field on singleSignOnSettings/password object.</span></span>|
|<span data-ttu-id="0e937-117">type</span><span class="sxs-lookup"><span data-stu-id="0e937-117">type</span></span>|<span data-ttu-id="0e937-118">String</span><span class="sxs-lookup"><span data-stu-id="0e937-118">String</span></span>|<span data-ttu-id="0e937-119">此凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="0e937-119">The type for this credential.</span></span> <span data-ttu-id="0e937-120">有效值：用户名、密码或其他。</span><span class="sxs-lookup"><span data-stu-id="0e937-120">Valid values: username, password, or other.</span></span>|
|<span data-ttu-id="0e937-121">value</span><span class="sxs-lookup"><span data-stu-id="0e937-121">value</span></span>|<span data-ttu-id="0e937-122">String</span><span class="sxs-lookup"><span data-stu-id="0e937-122">String</span></span>|<span data-ttu-id="0e937-123">此凭据的值。</span><span class="sxs-lookup"><span data-stu-id="0e937-123">The value for this credential.</span></span> <span data-ttu-id="0e937-124">例如，mysuperhiddenpassword。</span><span class="sxs-lookup"><span data-stu-id="0e937-124">e.g, mysuperhiddenpassword.</span></span> <span data-ttu-id="0e937-125">请注意，密码的值为仅写值，该值永远不能读回。</span><span class="sxs-lookup"><span data-stu-id="0e937-125">Note the value for passwords is write-only, the value can never be read back.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e937-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e937-126">JSON representation</span></span>

<span data-ttu-id="0e937-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e937-127">The following is a JSON representation of the resource.</span></span>

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


