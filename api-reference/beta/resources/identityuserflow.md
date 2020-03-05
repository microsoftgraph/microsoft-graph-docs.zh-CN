---
title: UserFlow 资源类型
description: 标识用户流是内置身份验证旅程
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4fa3064d19d96a2a8297f72de6a625ee36c8db3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496549"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="8a442-103">UserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="8a442-103">UserFlow resource type</span></span>

<span data-ttu-id="8a442-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8a442-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a442-105">用户流使您能够定义预定义的可配置策略，用于登录、注册、组合注册和登录、密码重置和配置文件更新。</span><span class="sxs-lookup"><span data-stu-id="8a442-105">User Flows enable you to define predefined, configurable policies for sign in, sign up, combined sign up and sign in, password reset and profile update.</span></span>

## <a name="methods"></a><span data-ttu-id="8a442-106">方法</span><span class="sxs-lookup"><span data-stu-id="8a442-106">Methods</span></span>

| <span data-ttu-id="8a442-107">方法</span><span class="sxs-lookup"><span data-stu-id="8a442-107">Method</span></span>       | <span data-ttu-id="8a442-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a442-108">Return Type</span></span> | <span data-ttu-id="8a442-109">说明</span><span class="sxs-lookup"><span data-stu-id="8a442-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8a442-110">List</span><span class="sxs-lookup"><span data-stu-id="8a442-110">List</span></span>](../api/identityuserflow-list.md) | <span data-ttu-id="8a442-111">[UserFlow](identityuserflow.md)集合</span><span class="sxs-lookup"><span data-stu-id="8a442-111">[UserFlow](identityuserflow.md) collection</span></span> | <span data-ttu-id="8a442-112">列出 UserFlows。</span><span class="sxs-lookup"><span data-stu-id="8a442-112">List UserFlows.</span></span> |
| [<span data-ttu-id="8a442-113">创建</span><span class="sxs-lookup"><span data-stu-id="8a442-113">Create</span></span>](../api/identityuserflow-post-userflows.md) | [<span data-ttu-id="8a442-114">UserFlow</span><span class="sxs-lookup"><span data-stu-id="8a442-114">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="8a442-115">创建 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="8a442-115">Create UserFlow object.</span></span> |
| [<span data-ttu-id="8a442-116">获取</span><span class="sxs-lookup"><span data-stu-id="8a442-116">Get</span></span>](../api/identityuserflow-get.md) | [<span data-ttu-id="8a442-117">UserFlow</span><span class="sxs-lookup"><span data-stu-id="8a442-117">UserFlow</span></span>](identityuserflow.md) | <span data-ttu-id="8a442-118">读取 UserFlow 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8a442-118">Read properties and relationships of UserFlow object.</span></span> |
| [<span data-ttu-id="8a442-119">删除</span><span class="sxs-lookup"><span data-stu-id="8a442-119">Delete</span></span>](../api/identityuserflow-delete.md) | <span data-ttu-id="8a442-120">无</span><span class="sxs-lookup"><span data-stu-id="8a442-120">None</span></span> | <span data-ttu-id="8a442-121">删除 UserFlow 对象。</span><span class="sxs-lookup"><span data-stu-id="8a442-121">Delete UserFlow object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a442-122">属性</span><span class="sxs-lookup"><span data-stu-id="8a442-122">Properties</span></span>

| <span data-ttu-id="8a442-123">属性</span><span class="sxs-lookup"><span data-stu-id="8a442-123">Property</span></span>     | <span data-ttu-id="8a442-124">类型</span><span class="sxs-lookup"><span data-stu-id="8a442-124">Type</span></span>        | <span data-ttu-id="8a442-125">说明</span><span class="sxs-lookup"><span data-stu-id="8a442-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8a442-126">id</span><span class="sxs-lookup"><span data-stu-id="8a442-126">id</span></span>|<span data-ttu-id="8a442-127">String</span><span class="sxs-lookup"><span data-stu-id="8a442-127">String</span></span>| <span data-ttu-id="8a442-128">只读。</span><span class="sxs-lookup"><span data-stu-id="8a442-128">Read-only.</span></span>|
|<span data-ttu-id="8a442-129">userFlowType</span><span class="sxs-lookup"><span data-stu-id="8a442-129">userFlowType</span></span>|<span data-ttu-id="8a442-130">string</span><span class="sxs-lookup"><span data-stu-id="8a442-130">string</span></span>| <span data-ttu-id="8a442-131">可取值为：`signUp`、`signIn`、`signUpOrSignIn`、`passwordReset`、`profileUpdate`、`resourceOwner` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8a442-131">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8a442-132">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="8a442-132">userFlowTypeVersion</span></span>|<span data-ttu-id="8a442-133">单精度</span><span class="sxs-lookup"><span data-stu-id="8a442-133">Single</span></span>| <span data-ttu-id="8a442-134">这是用户流类型的版本。</span><span class="sxs-lookup"><span data-stu-id="8a442-134">This is the version of the user flow type.</span></span> <span data-ttu-id="8a442-135">每个用户流类型都可以有不同的可能版本，如1、1.1 或2。</span><span class="sxs-lookup"><span data-stu-id="8a442-135">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="8a442-136">关系</span><span class="sxs-lookup"><span data-stu-id="8a442-136">Relationships</span></span>

<span data-ttu-id="8a442-137">无</span><span class="sxs-lookup"><span data-stu-id="8a442-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a442-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a442-138">JSON representation</span></span>

<span data-ttu-id="8a442-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a442-139">The following is a JSON representation of the resource.</span></span>

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
