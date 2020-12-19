---
title: invokeUserFlowListener 资源类型
description: 用于在身份验证事件期间调用用户流的侦听器。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0ca1c61d830a2ff98f2d72839129d75cc6287c36
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720153"
---
# <a name="invokeuserflowlistener-resource-type"></a><span data-ttu-id="05eaa-103">invokeUserFlowListener 资源类型</span><span class="sxs-lookup"><span data-stu-id="05eaa-103">invokeUserFlowListener resource type</span></span>

<span data-ttu-id="05eaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05eaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05eaa-105">你可以为[onSignUpStart 事件创建 invokeUserFlowListener。](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="05eaa-105">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event.</span></span> <span data-ttu-id="05eaa-106">这会将应用程序与用户流关联，从而启用应用程序的外部 [标识自助注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) 。</span><span class="sxs-lookup"><span data-stu-id="05eaa-106">This associates an application with a user flow, which enables [external identities self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) for the application.</span></span> <span data-ttu-id="05eaa-107">将应用程序与用户流关联后，转到该应用程序的用户将能够启动设置来宾帐户的注册流。</span><span class="sxs-lookup"><span data-stu-id="05eaa-107">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

<span data-ttu-id="05eaa-108">继承自抽象基类型 [authenticationListener](../resources/authenticationlistener.md)。</span><span class="sxs-lookup"><span data-stu-id="05eaa-108">Inherits from the abstract base type [authenticationListener](../resources/authenticationlistener.md).</span></span>

## <a name="properties"></a><span data-ttu-id="05eaa-109">属性</span><span class="sxs-lookup"><span data-stu-id="05eaa-109">Properties</span></span>

|<span data-ttu-id="05eaa-110">属性</span><span class="sxs-lookup"><span data-stu-id="05eaa-110">Property</span></span>|<span data-ttu-id="05eaa-111">类型</span><span class="sxs-lookup"><span data-stu-id="05eaa-111">Type</span></span>|<span data-ttu-id="05eaa-112">说明</span><span class="sxs-lookup"><span data-stu-id="05eaa-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05eaa-113">id</span><span class="sxs-lookup"><span data-stu-id="05eaa-113">id</span></span>|<span data-ttu-id="05eaa-114">String</span><span class="sxs-lookup"><span data-stu-id="05eaa-114">String</span></span>|<span data-ttu-id="05eaa-115">操作标识符。</span><span class="sxs-lookup"><span data-stu-id="05eaa-115">The identifier of the action.</span></span> <span data-ttu-id="05eaa-116">继承自 [authenticationListener](../resources/authenticationlistener.md)。</span><span class="sxs-lookup"><span data-stu-id="05eaa-116">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="05eaa-117">priority</span><span class="sxs-lookup"><span data-stu-id="05eaa-117">priority</span></span>|<span data-ttu-id="05eaa-118">Int32</span><span class="sxs-lookup"><span data-stu-id="05eaa-118">Int32</span></span>|<span data-ttu-id="05eaa-119">用于确定多个适用操作之一的操作的优先级。</span><span class="sxs-lookup"><span data-stu-id="05eaa-119">The priority of the action that is used to determine one out of multiple applicable actions.</span></span> <span data-ttu-id="05eaa-120">继承自 [authenticationListener](../resources/authenticationlistener.md)。</span><span class="sxs-lookup"><span data-stu-id="05eaa-120">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|
|<span data-ttu-id="05eaa-121">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="05eaa-121">sourceFilter</span></span>|[<span data-ttu-id="05eaa-122">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="05eaa-122">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="05eaa-123">基于用于确定是否执行侦听器的身份验证源进行筛选。</span><span class="sxs-lookup"><span data-stu-id="05eaa-123">Filter based on the source of the authentication that is used to determine whether the listener is executed.</span></span> <span data-ttu-id="05eaa-124">继承自 [authenticationListener](../resources/authenticationlistener.md)。</span><span class="sxs-lookup"><span data-stu-id="05eaa-124">Inherited from [authenticationListener](../resources/authenticationlistener.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="05eaa-125">关系</span><span class="sxs-lookup"><span data-stu-id="05eaa-125">Relationships</span></span>

|<span data-ttu-id="05eaa-126">关系</span><span class="sxs-lookup"><span data-stu-id="05eaa-126">Relationship</span></span>|<span data-ttu-id="05eaa-127">类型</span><span class="sxs-lookup"><span data-stu-id="05eaa-127">Type</span></span>|<span data-ttu-id="05eaa-128">说明</span><span class="sxs-lookup"><span data-stu-id="05eaa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05eaa-129">userFlow</span><span class="sxs-lookup"><span data-stu-id="05eaa-129">userFlow</span></span>|[<span data-ttu-id="05eaa-130">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="05eaa-130">b2xIdentityUserFlow</span></span>](../resources/b2xidentityuserflow.md)|<span data-ttu-id="05eaa-131">执行此操作时调用的用户流。</span><span class="sxs-lookup"><span data-stu-id="05eaa-131">The user flow that is invoked when this action executes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05eaa-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05eaa-132">JSON representation</span></span>

<span data-ttu-id="05eaa-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05eaa-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.invokeUserFlowListener",
  "baseType": "microsoft.graph.authenticationListener",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  },
  "userFlow": {
    "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
  }
}
```
