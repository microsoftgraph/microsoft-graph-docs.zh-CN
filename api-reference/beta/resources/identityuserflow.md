---
title: UserFlow 资源类型
description: 标识用户流是内置身份验证旅程
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0d76d7a2ab3516717d01f0371b84531e211181fd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016631"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="9514f-103">UserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="9514f-103">UserFlow resource type</span></span>

<span data-ttu-id="9514f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9514f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9514f-105">用户流使您能够定义预定义的可配置策略，用于登录、注册、组合注册和登录、密码重置和配置文件更新。</span><span class="sxs-lookup"><span data-stu-id="9514f-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="9514f-106">方法</span><span class="sxs-lookup"><span data-stu-id="9514f-106">Methods</span></span>

| <span data-ttu-id="9514f-107">方法</span><span class="sxs-lookup"><span data-stu-id="9514f-107">Method</span></span>       | <span data-ttu-id="9514f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9514f-108">Return Type</span></span> | <span data-ttu-id="9514f-109">Description</span><span class="sxs-lookup"><span data-stu-id="9514f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9514f-110">List</span><span class="sxs-lookup"><span data-stu-id="9514f-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="9514f-111">[UserFlow](identityuserflow.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9514f-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="9514f-112">列出 UserFlows。</span><span class="sxs-lookup"><span data-stu-id="9514f-112">List UserFlows.</span></span> |
| [<span data-ttu-id="9514f-113">创建</span><span class="sxs-lookup"><span data-stu-id="9514f-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="9514f-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="9514f-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="9514f-115">创建 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="9514f-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="9514f-116">获取</span><span class="sxs-lookup"><span data-stu-id="9514f-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="9514f-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="9514f-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="9514f-118">读取 UserFlow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9514f-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="9514f-119">删除</span><span class="sxs-lookup"><span data-stu-id="9514f-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="9514f-120">无</span><span class="sxs-lookup"><span data-stu-id="9514f-120">None</span></span> | <span data-ttu-id="9514f-121">删除 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="9514f-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9514f-122">属性</span><span class="sxs-lookup"><span data-stu-id="9514f-122">Properties</span></span>

| <span data-ttu-id="9514f-123">属性</span><span class="sxs-lookup"><span data-stu-id="9514f-123">Property</span></span>     | <span data-ttu-id="9514f-124">类型</span><span class="sxs-lookup"><span data-stu-id="9514f-124">Type</span></span>        | <span data-ttu-id="9514f-125">说明</span><span class="sxs-lookup"><span data-stu-id="9514f-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9514f-126">id</span><span class="sxs-lookup"><span data-stu-id="9514f-126">id</span></span>|<span data-ttu-id="9514f-127">String</span><span class="sxs-lookup"><span data-stu-id="9514f-127">String</span></span>| <span data-ttu-id="9514f-128">只读。</span><span class="sxs-lookup"><span data-stu-id="9514f-128">Read-only.</span></span>|
|<span data-ttu-id="9514f-129">userFlowType</span><span class="sxs-lookup"><span data-stu-id="9514f-129">userFlowType</span></span>|<span data-ttu-id="9514f-130">string</span><span class="sxs-lookup"><span data-stu-id="9514f-130">string</span></span>| <span data-ttu-id="9514f-131">可取值为：`signUp`、`signIn`、`signUpOrSignIn`、`passwordReset`、`profileUpdate`、`resourceOwner` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9514f-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9514f-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="9514f-132">userFlowTypeVersion</span></span>|<span data-ttu-id="9514f-133">单一</span><span class="sxs-lookup"><span data-stu-id="9514f-133">Single</span></span>| <span data-ttu-id="9514f-134">这是用户流类型的版本。</span><span class="sxs-lookup"><span data-stu-id="9514f-134">This is the version of the user flow type.</span></span> <span data-ttu-id="9514f-135">每个用户流类型都可以有不同的可能版本，如1、1.1 或2。</span><span class="sxs-lookup"><span data-stu-id="9514f-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="9514f-136">关系</span><span class="sxs-lookup"><span data-stu-id="9514f-136">Relationships</span></span>

<span data-ttu-id="9514f-137">无</span><span class="sxs-lookup"><span data-stu-id="9514f-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9514f-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9514f-138">JSON representation</span></span>

<span data-ttu-id="9514f-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9514f-139">The following is a JSON representation of the resource.</span></span>

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


