---
title: UserFlow 资源类型
description: 标识用户流是内置身份验证旅程
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4b4842b506e3c3c3e675ec2a47837fbf0c2e10be
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158287"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="77246-103">UserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="77246-103">UserFlow resource type</span></span>

<span data-ttu-id="77246-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77246-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77246-105">用户流使您能够定义预定义的可配置策略，用于登录、注册、组合注册和登录、密码重置和配置文件更新。</span><span class="sxs-lookup"><span data-stu-id="77246-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="77246-106">方法</span><span class="sxs-lookup"><span data-stu-id="77246-106">Methods</span></span>

| <span data-ttu-id="77246-107">方法</span><span class="sxs-lookup"><span data-stu-id="77246-107">Method</span></span>       | <span data-ttu-id="77246-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="77246-108">Return Type</span></span> | <span data-ttu-id="77246-109">Description</span><span class="sxs-lookup"><span data-stu-id="77246-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="77246-110">List</span><span class="sxs-lookup"><span data-stu-id="77246-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="77246-111">[UserFlow](identityuserflow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77246-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="77246-112">列出 UserFlows。</span><span class="sxs-lookup"><span data-stu-id="77246-112">List UserFlows.</span></span> |
| [<span data-ttu-id="77246-113">创建</span><span class="sxs-lookup"><span data-stu-id="77246-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="77246-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="77246-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="77246-115">创建 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="77246-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="77246-116">Get</span><span class="sxs-lookup"><span data-stu-id="77246-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="77246-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="77246-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="77246-118">读取 UserFlow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77246-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="77246-119">删除</span><span class="sxs-lookup"><span data-stu-id="77246-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="77246-120">无</span><span class="sxs-lookup"><span data-stu-id="77246-120">None</span></span> | <span data-ttu-id="77246-121">删除 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="77246-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="77246-122">属性</span><span class="sxs-lookup"><span data-stu-id="77246-122">Properties</span></span>

| <span data-ttu-id="77246-123">属性</span><span class="sxs-lookup"><span data-stu-id="77246-123">Property</span></span>     | <span data-ttu-id="77246-124">类型</span><span class="sxs-lookup"><span data-stu-id="77246-124">Type</span></span>        | <span data-ttu-id="77246-125">说明</span><span class="sxs-lookup"><span data-stu-id="77246-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="77246-126">id</span><span class="sxs-lookup"><span data-stu-id="77246-126">id</span></span>|<span data-ttu-id="77246-127">String</span><span class="sxs-lookup"><span data-stu-id="77246-127">String</span></span>| <span data-ttu-id="77246-128">只读。</span><span class="sxs-lookup"><span data-stu-id="77246-128">Read-only.</span></span>|
|<span data-ttu-id="77246-129">userFlowType</span><span class="sxs-lookup"><span data-stu-id="77246-129">userFlowType</span></span>|<span data-ttu-id="77246-130">string</span><span class="sxs-lookup"><span data-stu-id="77246-130">string</span></span>| <span data-ttu-id="77246-131">可取值为：`signUp`、`signIn`、`signUpOrSignIn`、`passwordReset`、`profileUpdate`、`resourceOwner` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="77246-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="77246-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="77246-132">userFlowTypeVersion</span></span>|<span data-ttu-id="77246-133">单一</span><span class="sxs-lookup"><span data-stu-id="77246-133">Single</span></span>| <span data-ttu-id="77246-134">这是用户流类型的版本。</span><span class="sxs-lookup"><span data-stu-id="77246-134">This is the version of the user flow type.</span></span> <span data-ttu-id="77246-135">每个用户流类型可以有不同的可能版本，如 1、1.1 或 2。</span><span class="sxs-lookup"><span data-stu-id="77246-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="77246-136">关系</span><span class="sxs-lookup"><span data-stu-id="77246-136">Relationships</span></span>

<span data-ttu-id="77246-137">无</span><span class="sxs-lookup"><span data-stu-id="77246-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77246-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77246-138">JSON representation</span></span>

<span data-ttu-id="77246-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77246-139">The following is a JSON representation of the resource.</span></span>

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


