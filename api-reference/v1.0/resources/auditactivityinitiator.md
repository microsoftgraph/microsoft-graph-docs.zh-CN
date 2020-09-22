---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起方可以是用户、应用程序或系统 (，它被视为应用程序) 。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8d6d4d41698e6251c0f33a637dff9e667df7d092
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988511"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="73866-104">auditActivityInitiator 资源类型</span><span class="sxs-lookup"><span data-stu-id="73866-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="73866-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73866-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73866-106">标识启动活动的资源对象。</span><span class="sxs-lookup"><span data-stu-id="73866-106">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="73866-107">发起方可以是用户、应用程序或系统 (，它被视为应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="73866-107">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="73866-108">属性</span><span class="sxs-lookup"><span data-stu-id="73866-108">Properties</span></span>

| <span data-ttu-id="73866-109">属性</span><span class="sxs-lookup"><span data-stu-id="73866-109">Property</span></span>     | <span data-ttu-id="73866-110">类型</span><span class="sxs-lookup"><span data-stu-id="73866-110">Type</span></span>   |<span data-ttu-id="73866-111">说明</span><span class="sxs-lookup"><span data-stu-id="73866-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73866-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="73866-112">app</span></span>|[<span data-ttu-id="73866-113">appIdentity</span><span class="sxs-lookup"><span data-stu-id="73866-113">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="73866-114">如果启动活动的资源是一个应用程序，则此属性指示所有与应用程序相关的信息，如 appId、Name、servicePrincipalId、Name。</span><span class="sxs-lookup"><span data-stu-id="73866-114">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="73866-115">user</span><span class="sxs-lookup"><span data-stu-id="73866-115">user</span></span>|[<span data-ttu-id="73866-116">userIdentity</span><span class="sxs-lookup"><span data-stu-id="73866-116">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="73866-117">如果启动活动的资源是用户，则此属性指示与用户相关的所有信息，如 userId、Name、UserPrinicpalName。</span><span class="sxs-lookup"><span data-stu-id="73866-117">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73866-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73866-118">JSON representation</span></span>

<span data-ttu-id="73866-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73866-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

