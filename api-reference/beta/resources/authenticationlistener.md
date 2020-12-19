---
title: authenticationListener 资源类型
description: 定义在身份验证事件期间要评估的侦听器。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d89d7660fc2580b8fad185633b6b819df1a41aaf
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720125"
---
# <a name="authenticationlistener-resource-type"></a><span data-ttu-id="216ca-103">authenticationListener 资源类型</span><span class="sxs-lookup"><span data-stu-id="216ca-103">authenticationListener resource type</span></span>

<span data-ttu-id="216ca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="216ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="216ca-105">定义在身份验证体验中发生身份验证事件时要评估的侦听器。</span><span class="sxs-lookup"><span data-stu-id="216ca-105">Defines a listener to be evaluate when an authentication event happens in an authentication experience.</span></span> <span data-ttu-id="216ca-106">authenticationListener 是抽象的，是您可以在身份验证事件期间评估的各种类型的侦听器的基类。</span><span class="sxs-lookup"><span data-stu-id="216ca-106">An authenticationListener is abstract and is the base class of the various types of listeners you can evaluate during an authentication event.</span></span> 

<span data-ttu-id="216ca-107">你可以为[onSignUpStart 事件创建 invokeUserFlowListener。](../resources/invokeuserflowlistener.md)</span><span class="sxs-lookup"><span data-stu-id="216ca-107">You can create an [invokeUserFlowListener](../resources/invokeuserflowlistener.md) for the onSignUpStart event..</span></span> <span data-ttu-id="216ca-108">这会将应用程序与用户流关联，从而启用自助服务 [注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) 过程。</span><span class="sxs-lookup"><span data-stu-id="216ca-108">This associates an application with a user flow, therefore enabling a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) process.</span></span> <span data-ttu-id="216ca-109">将应用程序与用户流关联后，转到该应用程序的用户将能够启动设置来宾帐户的注册流。</span><span class="sxs-lookup"><span data-stu-id="216ca-109">Once an application is associated with a user flow, users who go to that application will be able to initiate a sign-up flow that provisions a guest account.</span></span>

## <a name="methods"></a><span data-ttu-id="216ca-110">方法</span><span class="sxs-lookup"><span data-stu-id="216ca-110">Methods</span></span>

|<span data-ttu-id="216ca-111">方法</span><span class="sxs-lookup"><span data-stu-id="216ca-111">Method</span></span>|<span data-ttu-id="216ca-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="216ca-112">Return type</span></span>|<span data-ttu-id="216ca-113">说明</span><span class="sxs-lookup"><span data-stu-id="216ca-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="216ca-114">列出 onSignUpStart</span><span class="sxs-lookup"><span data-stu-id="216ca-114">List onSignUpStart</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="216ca-115">[authenticationListener](../resources/authenticationlistener.md) 集合</span><span class="sxs-lookup"><span data-stu-id="216ca-115">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="216ca-116">获取 onSignupStart 事件支持的 authenticationListener 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="216ca-116">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="216ca-117">创建 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-117">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="216ca-118">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-118">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="216ca-119">为 onSignupStart 事件创建新的 authenticationListener 对象。</span><span class="sxs-lookup"><span data-stu-id="216ca-119">Create a new authenticationListener object for the onSignupStart event.</span></span>|
|[<span data-ttu-id="216ca-120">更新 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-120">Update authenticationListener</span></span>](../api/authenticationlistener-update.md)|[<span data-ttu-id="216ca-121">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-121">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="216ca-122">更新为身份验证管道中的 onSignupStart 事件定义的指定侦听器。</span><span class="sxs-lookup"><span data-stu-id="216ca-122">Update the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="216ca-123">Put authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-123">Put authenticationListener</span></span>](../api/authenticationlistener-put.md)|[<span data-ttu-id="216ca-124">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-124">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="216ca-125">替换 authenticationListener 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="216ca-125">Replace the properties of an authenticationListener object.</span></span>|
|[<span data-ttu-id="216ca-126">获取 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-126">Get authenticationListener</span></span>](../api/authenticationlistener-get.md)|[<span data-ttu-id="216ca-127">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-127">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="216ca-128">获取为身份验证管道中的 onSignupStart 事件定义的指定侦听器。</span><span class="sxs-lookup"><span data-stu-id="216ca-128">Get the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|
|[<span data-ttu-id="216ca-129">删除 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="216ca-129">Delete authenticationListener</span></span>](../api/authenticationlistener-delete.md)|<span data-ttu-id="216ca-130">无</span><span class="sxs-lookup"><span data-stu-id="216ca-130">None</span></span>|<span data-ttu-id="216ca-131">删除为身份验证管道中的 onSignupStart 事件定义的指定侦听器。</span><span class="sxs-lookup"><span data-stu-id="216ca-131">Delete the specified listener defined for the onSignupStart event in the authentication pipeline.</span></span>|

## <a name="properties"></a><span data-ttu-id="216ca-132">属性</span><span class="sxs-lookup"><span data-stu-id="216ca-132">Properties</span></span>

|<span data-ttu-id="216ca-133">属性</span><span class="sxs-lookup"><span data-stu-id="216ca-133">Property</span></span>|<span data-ttu-id="216ca-134">类型</span><span class="sxs-lookup"><span data-stu-id="216ca-134">Type</span></span>|<span data-ttu-id="216ca-135">说明</span><span class="sxs-lookup"><span data-stu-id="216ca-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="216ca-136">id</span><span class="sxs-lookup"><span data-stu-id="216ca-136">id</span></span>|<span data-ttu-id="216ca-137">String</span><span class="sxs-lookup"><span data-stu-id="216ca-137">String</span></span>|<span data-ttu-id="216ca-138">操作标识符。</span><span class="sxs-lookup"><span data-stu-id="216ca-138">The identifier of the action.</span></span>|
|<span data-ttu-id="216ca-139">priority</span><span class="sxs-lookup"><span data-stu-id="216ca-139">priority</span></span>|<span data-ttu-id="216ca-140">Int32</span><span class="sxs-lookup"><span data-stu-id="216ca-140">Int32</span></span>|<span data-ttu-id="216ca-141">侦听器的优先级。</span><span class="sxs-lookup"><span data-stu-id="216ca-141">The priority of the listener.</span></span> <span data-ttu-id="216ca-142">确定事件具有多个侦听器时的评估顺序。</span><span class="sxs-lookup"><span data-stu-id="216ca-142">Determines the order of evaluation when an event has multiple listeners.</span></span> <span data-ttu-id="216ca-143">优先级从低到高计算。</span><span class="sxs-lookup"><span data-stu-id="216ca-143">The priority is evaluated from low to high.</span></span>|
|<span data-ttu-id="216ca-144">sourceFilter</span><span class="sxs-lookup"><span data-stu-id="216ca-144">sourceFilter</span></span>|[<span data-ttu-id="216ca-145">authenticationSourceFilter</span><span class="sxs-lookup"><span data-stu-id="216ca-145">authenticationSourceFilter</span></span>](../resources/authenticationsourcefilter.md)|<span data-ttu-id="216ca-146">基于用于确定是否评估侦听器的身份验证源进行筛选。</span><span class="sxs-lookup"><span data-stu-id="216ca-146">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span> <span data-ttu-id="216ca-147">当前仅限于基于用户进行身份验证的应用程序的评估。</span><span class="sxs-lookup"><span data-stu-id="216ca-147">This is currently limited to evaluations based on application the user is authenticating to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="216ca-148">关系</span><span class="sxs-lookup"><span data-stu-id="216ca-148">Relationships</span></span>

<span data-ttu-id="216ca-149">无。</span><span class="sxs-lookup"><span data-stu-id="216ca-149">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="216ca-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="216ca-150">JSON representation</span></span>

<span data-ttu-id="216ca-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="216ca-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationListener",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "priority": "Integer",
  "sourceFilter": {
    "@odata.type": "microsoft.graph.authenticationSourceFilter"
  }
}
```
