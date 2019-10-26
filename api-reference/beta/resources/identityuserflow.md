---
title: UserFlow 资源类型
description: 标识用户流是内置身份验证旅程
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5410b65dfdb0841aa997022b43dc04d0a4627008
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734540"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="bb6f4-103">UserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb6f4-103">UserFlow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb6f4-104">用户流使您能够定义预定义的可配置策略，用于登录、注册、组合注册和登录、密码重置和配置文件更新。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-104">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="bb6f4-105">方法</span><span class="sxs-lookup"><span data-stu-id="bb6f4-105">Methods</span></span>

| <span data-ttu-id="bb6f4-106">方法</span><span class="sxs-lookup"><span data-stu-id="bb6f4-106">Method</span></span>       | <span data-ttu-id="bb6f4-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb6f4-107">Return Type</span></span> | <span data-ttu-id="bb6f4-108">说明</span><span class="sxs-lookup"><span data-stu-id="bb6f4-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="bb6f4-109">List</span><span class="sxs-lookup"><span data-stu-id="bb6f4-109">List</span></span>](../api/identityuserflow-list.md) | [<span data-ttu-id="bb6f4-110">UserFlow</span><span class="sxs-lookup"><span data-stu-id="bb6f4-110">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="bb6f4-111">列出 UserFlows。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-111">List UserFlows.</span></span> |
| [<span data-ttu-id="bb6f4-112">创建</span><span class="sxs-lookup"><span data-stu-id="bb6f4-112">Create</span></span>](../api/identityuserflow-post-userflows.md) | <span data-ttu-id="bb6f4-113">无</span><span class="sxs-lookup"><span data-stu-id="bb6f4-113">None</span></span> | <span data-ttu-id="bb6f4-114">创建 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-114">Create UserFlow object.</span></span> |
| [<span data-ttu-id="bb6f4-115">获取</span><span class="sxs-lookup"><span data-stu-id="bb6f4-115">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="bb6f4-116">UserFlow</span><span class="sxs-lookup"><span data-stu-id="bb6f4-116">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="bb6f4-117">读取 UserFlow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-117">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="bb6f4-118">删除</span><span class="sxs-lookup"><span data-stu-id="bb6f4-118">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="bb6f4-119">无</span><span class="sxs-lookup"><span data-stu-id="bb6f4-119">None</span></span> | <span data-ttu-id="bb6f4-120">删除 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-120">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="bb6f4-121">属性</span><span class="sxs-lookup"><span data-stu-id="bb6f4-121">Properties</span></span>

| <span data-ttu-id="bb6f4-122">属性</span><span class="sxs-lookup"><span data-stu-id="bb6f4-122">Property</span></span>     | <span data-ttu-id="bb6f4-123">类型</span><span class="sxs-lookup"><span data-stu-id="bb6f4-123">Type</span></span>        | <span data-ttu-id="bb6f4-124">说明</span><span class="sxs-lookup"><span data-stu-id="bb6f4-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb6f4-125">id</span><span class="sxs-lookup"><span data-stu-id="bb6f4-125">id</span></span>|<span data-ttu-id="bb6f4-126">String</span><span class="sxs-lookup"><span data-stu-id="bb6f4-126">String</span></span>| <span data-ttu-id="bb6f4-127">只读。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-127">Read-only.</span></span>|
|<span data-ttu-id="bb6f4-128">userFlowType</span><span class="sxs-lookup"><span data-stu-id="bb6f4-128">userFlowType</span></span>|<span data-ttu-id="bb6f4-129">string</span><span class="sxs-lookup"><span data-stu-id="bb6f4-129">string</span></span>| <span data-ttu-id="bb6f4-130">可取值为：`signUp`、`signIn`、`signUpOrSignIn`、`passwordReset`、`profileUpdate`、`resourceOwner` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-130">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bb6f4-131">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="bb6f4-131">userFlowTypeVersion</span></span>|<span data-ttu-id="bb6f4-132">单精度</span><span class="sxs-lookup"><span data-stu-id="bb6f4-132">Single</span></span>| <span data-ttu-id="bb6f4-133">这是用户流类型的版本。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-133">This is the version of the user flow type.</span></span> <span data-ttu-id="bb6f4-134">每个用户流类型都可以有不同的可能版本，如1、1.1 或2。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-134">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="bb6f4-135">关系</span><span class="sxs-lookup"><span data-stu-id="bb6f4-135">Relationships</span></span>

<span data-ttu-id="bb6f4-136">无</span><span class="sxs-lookup"><span data-stu-id="bb6f4-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb6f4-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb6f4-137">JSON representation</span></span>

<span data-ttu-id="bb6f4-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb6f4-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.UserFlow",
  "baseType": "",
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
