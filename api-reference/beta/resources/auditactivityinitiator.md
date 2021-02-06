---
title: auditActivityInitiator 资源类型
description: '标识启动活动的资源对象。 发起人可以是用户、应用或系统 (被视为应用) '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
author: SarahBar
ms.openlocfilehash: 71aa5e2bd09d66a2aea49058ceffea3e017eaf4d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131633"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="85a24-104">auditActivityInitiator 资源类型</span><span class="sxs-lookup"><span data-stu-id="85a24-104">auditActivityInitiator resource type</span></span>

<span data-ttu-id="85a24-105">命名空间：microsoft.graph 标识启动活动的资源对象。</span><span class="sxs-lookup"><span data-stu-id="85a24-105">Namespace: microsoft.graph Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="85a24-106">发起人可以是用户、应用或系统 (被视为应用) </span><span class="sxs-lookup"><span data-stu-id="85a24-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="85a24-107">属性</span><span class="sxs-lookup"><span data-stu-id="85a24-107">Properties</span></span>
| <span data-ttu-id="85a24-108">属性</span><span class="sxs-lookup"><span data-stu-id="85a24-108">Property</span></span>     | <span data-ttu-id="85a24-109">类型</span><span class="sxs-lookup"><span data-stu-id="85a24-109">Type</span></span>   |<span data-ttu-id="85a24-110">说明</span><span class="sxs-lookup"><span data-stu-id="85a24-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85a24-111">应用</span><span class="sxs-lookup"><span data-stu-id="85a24-111">app</span></span>|[<span data-ttu-id="85a24-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="85a24-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="85a24-113">如果启动活动的资源是应用，则此属性指示 appId、Name、servicePrincipalId、Name 等所有应用相关信息。</span><span class="sxs-lookup"><span data-stu-id="85a24-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="85a24-114">user</span><span class="sxs-lookup"><span data-stu-id="85a24-114">user</span></span>|[<span data-ttu-id="85a24-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="85a24-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="85a24-116">如果启动活动的资源是用户，则此属性指示与用户 Id、名称、UserPrinicpalName 等所有用户相关信息。</span><span class="sxs-lookup"><span data-stu-id="85a24-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85a24-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85a24-117">JSON representation</span></span>

<span data-ttu-id="85a24-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85a24-118">Here is a JSON representation of the resource.</span></span>

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


