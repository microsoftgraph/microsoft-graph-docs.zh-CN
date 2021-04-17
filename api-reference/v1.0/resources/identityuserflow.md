---
title: UserFlow 资源类型
description: 表示内置身份验证旅程中包含的标识用户流。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4e03faaff265bf82bacf16a2db6c75e81176eafa
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882809"
---
# <a name="userflow-resource-type"></a><span data-ttu-id="01fc6-103">UserFlow 资源类型</span><span class="sxs-lookup"><span data-stu-id="01fc6-103">UserFlow resource type</span></span>

<span data-ttu-id="01fc6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01fc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01fc6-105">用户流使您能够为登录、注册、组合注册和登录、密码重置和配置文件更新定义预定义的可配置策略。</span><span class="sxs-lookup"><span data-stu-id="01fc6-105">User Flows enable you to define predefined, configurable policies for sign-in, sign-up, combined sign-up and sign-in, password reset, and profile update.</span></span> <span data-ttu-id="01fc6-106">这是其他用户流从其继承的基类。</span><span class="sxs-lookup"><span data-stu-id="01fc6-106">This is a base class that other user flows inherit from.</span></span>

## <a name="properties"></a><span data-ttu-id="01fc6-107">属性</span><span class="sxs-lookup"><span data-stu-id="01fc6-107">Properties</span></span>

| <span data-ttu-id="01fc6-108">属性</span><span class="sxs-lookup"><span data-stu-id="01fc6-108">Property</span></span>     | <span data-ttu-id="01fc6-109">类型</span><span class="sxs-lookup"><span data-stu-id="01fc6-109">Type</span></span>        | <span data-ttu-id="01fc6-110">说明</span><span class="sxs-lookup"><span data-stu-id="01fc6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="01fc6-111">id</span><span class="sxs-lookup"><span data-stu-id="01fc6-111">id</span></span>|<span data-ttu-id="01fc6-112">String</span><span class="sxs-lookup"><span data-stu-id="01fc6-112">String</span></span>| <span data-ttu-id="01fc6-113">用户流的标识符。</span><span class="sxs-lookup"><span data-stu-id="01fc6-113">The identifier of the user flow.</span></span> <span data-ttu-id="01fc6-114">将 **B2C_1_** 前缀添加到您提供的值中。</span><span class="sxs-lookup"><span data-stu-id="01fc6-114">The prefix of **B2C_1_** is added to the value that you provide.</span></span>|
|<span data-ttu-id="01fc6-115">userFlowType</span><span class="sxs-lookup"><span data-stu-id="01fc6-115">userFlowType</span></span>|<span data-ttu-id="01fc6-116">userFlowType</span><span class="sxs-lookup"><span data-stu-id="01fc6-116">userFlowType</span></span>| <span data-ttu-id="01fc6-117">可取值为：`signUp`、`signIn`、`signUpOrSignIn`、`passwordReset`、`profileUpdate`、`resourceOwner` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="01fc6-117">Possible values are: `signUp`, `signIn`, `signUpOrSignIn`, `passwordReset`, `profileUpdate`, `resourceOwner`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="01fc6-118">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="01fc6-118">userFlowTypeVersion</span></span>|<span data-ttu-id="01fc6-119">单一</span><span class="sxs-lookup"><span data-stu-id="01fc6-119">Single</span></span>| <span data-ttu-id="01fc6-120">这是用户流类型的版本。</span><span class="sxs-lookup"><span data-stu-id="01fc6-120">This is the version of the user flow type.</span></span> <span data-ttu-id="01fc6-121">每个用户流类型可能具有不同的版本，如 1、1.1 或 2。</span><span class="sxs-lookup"><span data-stu-id="01fc6-121">Each user flow type can have different possible versions such as 1, 1.1 or 2.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="01fc6-122">关系</span><span class="sxs-lookup"><span data-stu-id="01fc6-122">Relationships</span></span>

<span data-ttu-id="01fc6-123">无</span><span class="sxs-lookup"><span data-stu-id="01fc6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01fc6-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01fc6-124">JSON representation</span></span>

<span data-ttu-id="01fc6-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01fc6-125">The following is a JSON representation of the resource.</span></span>

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
