---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起人可以是用户、应用或系统 (被视为应用) 。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fbc2fd2f6c93cac583fc1ec28375d8538d35b447
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135756"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="89e4f-104">auditActivityInitiator 资源类型</span><span class="sxs-lookup"><span data-stu-id="89e4f-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="89e4f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e4f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="89e4f-106">标识启动活动的资源对象。</span><span class="sxs-lookup"><span data-stu-id="89e4f-106">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="89e4f-107">发起人可以是用户、应用或系统 (被视为应用) 。</span><span class="sxs-lookup"><span data-stu-id="89e4f-107">The initiator can be a user, an app, or a system (which is considered an app).</span></span>

## <a name="properties"></a><span data-ttu-id="89e4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="89e4f-108">Properties</span></span>

| <span data-ttu-id="89e4f-109">属性</span><span class="sxs-lookup"><span data-stu-id="89e4f-109">Property</span></span>     | <span data-ttu-id="89e4f-110">类型</span><span class="sxs-lookup"><span data-stu-id="89e4f-110">Type</span></span>   |<span data-ttu-id="89e4f-111">说明</span><span class="sxs-lookup"><span data-stu-id="89e4f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89e4f-112">应用</span><span class="sxs-lookup"><span data-stu-id="89e4f-112">app</span></span>|[<span data-ttu-id="89e4f-113">appIdentity</span><span class="sxs-lookup"><span data-stu-id="89e4f-113">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="89e4f-114">如果启动活动的资源是应用，则此属性指示 appId、Name、servicePrincipalId、Name 等所有应用相关信息。</span><span class="sxs-lookup"><span data-stu-id="89e4f-114">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="89e4f-115">user</span><span class="sxs-lookup"><span data-stu-id="89e4f-115">user</span></span>|[<span data-ttu-id="89e4f-116">userIdentity</span><span class="sxs-lookup"><span data-stu-id="89e4f-116">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="89e4f-117">如果启动活动的资源是用户，则此属性指示与用户 Id、名称、UserPrinicpalName 等所有用户相关信息。</span><span class="sxs-lookup"><span data-stu-id="89e4f-117">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89e4f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89e4f-118">JSON representation</span></span>

<span data-ttu-id="89e4f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89e4f-119">Here is a JSON representation of the resource.</span></span>

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

