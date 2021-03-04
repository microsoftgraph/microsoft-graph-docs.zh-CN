---
title: UserFlow 资源类型
description: 标识用户流是内置身份验证旅程
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3a5cb0bfd61e9b99e9837c36484feefc0ff3a635
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440246"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="b2891-103">UserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="b2891-103">UserFlow resource type</span></span>

<span data-ttu-id="b2891-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2891-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2891-105">用户流使您能够为登录、注册、组合注册和登录、密码重置和配置文件更新定义预定义的可配置策略。</span><span class="sxs-lookup"><span data-stu-id="b2891-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="b2891-106">Methods</span><span class="sxs-lookup"><span data-stu-id="b2891-106">Methods</span></span>

| <span data-ttu-id="b2891-107">方法</span><span class="sxs-lookup"><span data-stu-id="b2891-107">Method</span></span>       | <span data-ttu-id="b2891-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b2891-108">Return Type</span></span> | <span data-ttu-id="b2891-109">Description</span><span class="sxs-lookup"><span data-stu-id="b2891-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b2891-110">List</span><span class="sxs-lookup"><span data-stu-id="b2891-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="b2891-111">[UserFlow](identityuserflow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b2891-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="b2891-112">列出 UserFlows。</span><span class="sxs-lookup"><span data-stu-id="b2891-112">List UserFlows.</span></span> |
| [<span data-ttu-id="b2891-113">创建</span><span class="sxs-lookup"><span data-stu-id="b2891-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="b2891-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="b2891-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="b2891-115">创建 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="b2891-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="b2891-116">获取</span><span class="sxs-lookup"><span data-stu-id="b2891-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="b2891-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="b2891-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="b2891-118">读取 UserFlow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b2891-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="b2891-119">删除</span><span class="sxs-lookup"><span data-stu-id="b2891-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="b2891-120">无</span><span class="sxs-lookup"><span data-stu-id="b2891-120">None</span></span> | <span data-ttu-id="b2891-121">删除 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="b2891-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b2891-122">属性</span><span class="sxs-lookup"><span data-stu-id="b2891-122">Properties</span></span>

| <span data-ttu-id="b2891-123">属性</span><span class="sxs-lookup"><span data-stu-id="b2891-123">Property</span></span>     | <span data-ttu-id="b2891-124">类型</span><span class="sxs-lookup"><span data-stu-id="b2891-124">Type</span></span>        | <span data-ttu-id="b2891-125">说明</span><span class="sxs-lookup"><span data-stu-id="b2891-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b2891-126">id</span><span class="sxs-lookup"><span data-stu-id="b2891-126">id</span></span>|<span data-ttu-id="b2891-127">String</span><span class="sxs-lookup"><span data-stu-id="b2891-127">String</span></span>| <span data-ttu-id="b2891-128">用户流的标识符。</span><span class="sxs-lookup"><span data-stu-id="b2891-128">The identifier of the user flow.</span></span> <span data-ttu-id="b2891-129">前缀 **B2C_1_添加到** 您提供的值。</span><span class="sxs-lookup"><span data-stu-id="b2891-129">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="b2891-130">userFlowType</span><span class="sxs-lookup"><span data-stu-id="b2891-130">userFlowType</span></span>|<span data-ttu-id="b2891-131">string</span><span class="sxs-lookup"><span data-stu-id="b2891-131">string</span></span>| <span data-ttu-id="b2891-132">可取值为：`signUp`、`signIn`、`signUpOrSignIn`、`passwordReset`、`profileUpdate`、`resourceOwner` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b2891-132">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b2891-133">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="b2891-133">userFlowTypeVersion</span></span>|<span data-ttu-id="b2891-134">单一</span><span class="sxs-lookup"><span data-stu-id="b2891-134">Single</span></span>| <span data-ttu-id="b2891-135">这是用户流类型的版本。</span><span class="sxs-lookup"><span data-stu-id="b2891-135">This is the version of the user flow type.</span></span> <span data-ttu-id="b2891-136">每个用户流类型可以具有不同的可能版本，如 1、1.1 或 2。</span><span class="sxs-lookup"><span data-stu-id="b2891-136">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="b2891-137">关系</span><span class="sxs-lookup"><span data-stu-id="b2891-137">Relationships</span></span>

<span data-ttu-id="b2891-138">无</span><span class="sxs-lookup"><span data-stu-id="b2891-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2891-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b2891-139">JSON representation</span></span>

<span data-ttu-id="b2891-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b2891-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "userFlowType": "string",
  "userFlowTypeVersion": "Single"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UserFlow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


