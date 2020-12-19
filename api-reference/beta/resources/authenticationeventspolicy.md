---
title: authenticationEventsPolicy 资源类型
description: 身份验证事件用于在身份验证流中的特定点调用用户流。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cc8789fb0de21980571bdcb5254a7760045e61b0
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720126"
---
# <a name="authenticationeventspolicy-resource-type"></a><span data-ttu-id="e6ffb-103">authenticationEventsPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6ffb-103">authenticationEventsPolicy resource type</span></span>

<span data-ttu-id="e6ffb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ffb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ffb-105">一个指定身份验证体验中的事件的资源，每个事件进一步定义可针对事件创建的可用侦听器类型。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-105">A resource that specifies the events in the authentication experience, with each event further defining the available types of listeners that can be created for the event.</span></span> <span data-ttu-id="e6ffb-106">事件是身份验证体验固有的;此资源不可由用户配置。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-106">Events are inherent to the authentication experience; this resource is not user configurable.</span></span>

## <a name="methods"></a><span data-ttu-id="e6ffb-107">方法</span><span class="sxs-lookup"><span data-stu-id="e6ffb-107">Methods</span></span>

|<span data-ttu-id="e6ffb-108">方法</span><span class="sxs-lookup"><span data-stu-id="e6ffb-108">Method</span></span>|<span data-ttu-id="e6ffb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6ffb-109">Return type</span></span>|<span data-ttu-id="e6ffb-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6ffb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6ffb-111">列出 onSignUpStart 侦听器</span><span class="sxs-lookup"><span data-stu-id="e6ffb-111">List onSignUpStart listeners</span></span>](../api/authenticationeventspolicy-list-onsignupstart.md)|<span data-ttu-id="e6ffb-112">[authenticationListener](../resources/authenticationlistener.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6ffb-112">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="e6ffb-113">获取 onSignupStart 事件支持的 authenticationListener 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-113">Get the collection of authenticationListener resources supported by the onSignupStart event.</span></span>|
|[<span data-ttu-id="e6ffb-114">创建 authenticationListener</span><span class="sxs-lookup"><span data-stu-id="e6ffb-114">Create authenticationListener</span></span>](../api/authenticationeventspolicy-post-onsignupstart.md)|[<span data-ttu-id="e6ffb-115">authenticationListener</span><span class="sxs-lookup"><span data-stu-id="e6ffb-115">authenticationListener</span></span>](../resources/authenticationlistener.md)|<span data-ttu-id="e6ffb-116">为 onSignupStart 事件创建新的 authenticationListener 对象。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-116">Create a new authenticationListener object for the onSignupStart event.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6ffb-117">属性</span><span class="sxs-lookup"><span data-stu-id="e6ffb-117">Properties</span></span>

|<span data-ttu-id="e6ffb-118">属性</span><span class="sxs-lookup"><span data-stu-id="e6ffb-118">Property</span></span>|<span data-ttu-id="e6ffb-119">类型</span><span class="sxs-lookup"><span data-stu-id="e6ffb-119">Type</span></span>|<span data-ttu-id="e6ffb-120">说明</span><span class="sxs-lookup"><span data-stu-id="e6ffb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ffb-121">id</span><span class="sxs-lookup"><span data-stu-id="e6ffb-121">id</span></span>|<span data-ttu-id="e6ffb-122">String</span><span class="sxs-lookup"><span data-stu-id="e6ffb-122">String</span></span>|<span data-ttu-id="e6ffb-123">策略的标识符。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-123">The identifier of the policy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6ffb-124">关系</span><span class="sxs-lookup"><span data-stu-id="e6ffb-124">Relationships</span></span>

|<span data-ttu-id="e6ffb-125">关系</span><span class="sxs-lookup"><span data-stu-id="e6ffb-125">Relationship</span></span>|<span data-ttu-id="e6ffb-126">类型</span><span class="sxs-lookup"><span data-stu-id="e6ffb-126">Type</span></span>|<span data-ttu-id="e6ffb-127">说明</span><span class="sxs-lookup"><span data-stu-id="e6ffb-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6ffb-128">onSignupStart</span><span class="sxs-lookup"><span data-stu-id="e6ffb-128">onSignupStart</span></span>|<span data-ttu-id="e6ffb-129">[authenticationListener](../resources/authenticationlistener.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e6ffb-129">[authenticationListener](../resources/authenticationlistener.md) collection</span></span>|<span data-ttu-id="e6ffb-130">注册时要采取的适用操作的列表。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-130">A list of applicable actions to be taken on sign-up.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6ffb-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6ffb-131">JSON representation</span></span>

<span data-ttu-id="e6ffb-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6ffb-132">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationEventsPolicy",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationEventsPolicy",
  "id": "String (identifier)"
}
```
